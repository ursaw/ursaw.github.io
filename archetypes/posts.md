+++
title = "{{ replace .Name "-" " " | title }}"
date = {{ .Date }}
tags = []
draft = true
+++


## New Cool Posts

{{ range first 10 ( where .Site.RegularPages "Type" "cool" ) }}
* {{ .Title }}
{{ end }}
