+++
title = "Python dataclasses"
date = 2022-03-18T13:42:12+01:00
tags = ["python"]
draft = false
+++

## Background
Although I work quite much with python I really hate the aspect of dynamically typing when using classes. In my opinion you should do on object oriented modelling to define attributes instead of adding attributes during runtime. 

I would like to have something like [perls use strict](https://perldoc.perl.org/strict) to at least define the attributes, even if the datatype is missing there. 

Python 3.7, [pep 557](https://peps.python.org/pep-0557/) introduced [dataclasses](https://docs.python.org/3/library/dataclasses.html) to the 
default library, which enables the developer to do an object oriented modelling with python. Additionally [dataclass_json](https://github.com/lidatong/dataclasses-json) is a simple addition to serialize dataclasses to json files. 


## Notes to the example
Never use the `__init__` method, this is generated internally, instead use the [`__post_init__`](https://docs.python.org/3/library/dataclasses.html#post-init-processing)  method optionally with `InitVar` attributes. You wont see the `InitVar` attributes in the JSON file.


## Implementation example

### code
```python
from dataclasses import dataclass, field, InitVar
from dataclasses_json import dataclass_json
from typing import List, Dict

import json

@dataclass_json
@dataclass
class AnotherClass:
    a_integer_att: int = field(default=None)

@dataclass_json
@dataclass
class ExampleClass:
    """Simple Example class with reference to another class."""
    identificator: str = field(default=None)

    a_list_of_strings: List[str] = field(default_factory=list)
    """List[str]: A list of strings."""

    a_dict_of_objects: Dict[str, AnotherClass] = field(default_factory=dict)
    """Dict[str, Field]: A dictionary of objects of AnotherClass."""

    a_helper: InitVar[str] = None

    def __post_init__(self, a_helper):
        print(
            f"post init is called from generated (never overwrite it!) card.__init__() with a_helper='{a_helper}'")

if __name__ == '__main__':
    print("card with constructor in main.")
    ea = ExampleClass("id01", a_dict_of_objects={"a": AnotherClass(1), "b": AnotherClass(99)}, a_helper="hey ho!")
    outfile_name = r"C:\temp\dataclass_example.json"
    
    print(f" * original id of object is {id(ea)}")
    # writing
    with open(outfile_name, 'w') as file:
           json.dump(ea.to_dict(), file, indent=2)

    # reading
    with open(outfile_name, 'r') as file:
        object_as_json = json.load(file)
        print("object from json file.")
        ea = ExampleClass.from_dict(object_as_json)
```

### Serialization
```json
{
  "identificator": "id01",
  "a_list_of_strings": [],
  "a_dict_of_objects": {
    "a": {
      "a_integer_att": 1
    },
    "b": {
      "a_integer_att": 99
    }
  }
}
```

