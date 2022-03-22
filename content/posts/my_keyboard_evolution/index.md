+++
title = "My Keyboard Evolution"
date = 2022-03-18T15:34:57+01:00
tags = ['keyboards']
draft = true
+++


## TL;DR
This is my historically ordered journey into ergonomic keyboards. I try to explain the background of the reasons for their choice, the advantages and limitations.

My main work on computers is coding, and I like terminals/consoles and try avoid using the mouse as much as possible.

From IBM model M to dactyl split ortho keyboard for ergonomics and fun. I am still an QWERTY but slowly moving to [COLMAK DH](https://colemakmods.github.io/mod-dh/keyboards.html#matrix-keyboards).

It was an evolution with multiple small changes, today I advice for the fast jump into an split ortho keyboard.


## IBM model M
{{< refphotos photo="kb_yacobo"  opts="250x" >}} 
I directly started my computer life at university with the [IBM model M](https://en.wikipedia.org/wiki/Model_M_keyboard) on workstations. 
I was lucky enough to get one of these keyboards and really liked it, the sound (first and foremost to mention), the feel, the size and the aura.
Luckily, Colleagues endured the keyboard. 

By the time I couldn't use it any longer, because of the PS2 adapter and the missing META key. The META key sounds odd, but I am used to re-arrange windows  in combination with cursor keys. 

In 2018 I bought a [Soarer's Converter](https://deskthority.net/viewtopic.php?f=7&t=2510&start=) to have an programmable USB adapter, where I exchanged the Pause key to the META key. I think I never used the Pause key in the last 20 years...

I switched to a large company with an open-plan office and left the model M at home. 

Interestingly, recently I pimped the model M with an [yacobo](https://github.com/sje-mse/yacobo) replacement controller to have an internal USB connection and fully programmable [QMK](https://docs.qmk.fm) support.


## Matias Ergopro
The [mathias ergopro](https://matias.ca/ergopro/pc/) was my first split keyboard,  I bought it used. I really liked the [quite click](https://matias.ca/switches/quiet/) switches and the ability to tent with the nice palm rests. 
My keyboard suffered from the ergopro disease of multiple key registers every now and then. Since I loved this keyboard, I always forgave it for this.

As time went on, I didn't feel comfortable with this keyboard anymore because I switched from the German to the American key layout and especially I wanted to go more ergo and try an ortho split. 


## Testing boards




### Ergodox
* cherry red
  
As the next step I got myself another used keyboard and thought the [ergodox](https://www.ergodox.io/) would be the one for me. I liked to think about the key layout and played around with [oryx](https://configure.zsa.io/ergodox-ez/layouts/default/latest/0). I was excited to flush it with [wally](https://ergodox-ez.com/pages/wally) because I was afraid I might brick it. 
But in the end I was shocked to find that I was not able to type with it at all.

The ortho layout and especially the thumb cluster was so unfamiliar to my fingers that I was unable to type the right keys. My bad typing habits from row staggered didn't work on the column staggered keyboard, so it wasn't fun to use at all. 

I ended up selling it again. After a few more experiences, I realized that I should have had more typing experience on [keybr](https://keybr.com) to give the ergodox a change. 



### DZ60 
* Gateron Browns
  
After the short ortho experiment I selected a DZ60 to switch 60% and to [US international](https://en.wikipedia.org/wiki/QWERTY#US-International) keyboard layout. This was the first time for me to compile [QMK](https://docs.qmk.fm) on Linux. I felt surprisingly comfortable with this board and with all layers. I bought myself an solder iron an modified the backspace key to a [HHKB](https://www.hhkeyboard.com/d) layout, because this is the part I really like at HHKB, while I dont understand the concept of the missing control keys.

## keebio Quefrency rev2

{{< refphotos photo="kb_quefrency"  opts="250x" >}} 

* Zealios Switch (V2) 62g


Since I was comfortable with 60% and missing the spilt, it was quite obvious for me that I need to build my first keeb which was a [quefrency](https://keeb.io/collections/quefrency-split-staggered-65-keyboard). First I waited for Rev 2 to come out, then I waited for the German vendor [candykeys](https://candykeys.com/) to have it. That took quite a while, but I got a good idea that an important part of building keyboards is waiting for parts.

I messed up the soldering and had to rebuild one half, which means waiting for parts again...

In the end I used it for a very short period, because I started to go to ortho layout. 
I like the keyboard very much because it is an smart interpretation of a split 60%, but for a while now, I think of selling...

## Sofle V1

{{< refphotos photo="kb_sofle"  opts="250x" >}} 

* [Sofle V1](https://josefadamcik.github.io/SofleKeyboard/)
* Zealios Switch (V2) 67g or Kaihl White

For my second built I dared a more complex build, and it take a while for me to get used to solder SMD diods. I already summarized my [first impression](/posts/thoughts_soflev1) of the Sofle, and this is the keyboard I have used most often (besides the [model M](#ibm-model-m)).

Most of the following builds are like 4x6+4 boards to me, as I can't live so far with fewer keys.

### Design Error
The Sofle has a small design flaw for which I have no solution. 

If you follow the key press, you hit the switch, which is mounted in the switch plate. The plate is connected with stand-offs to the back plate, which is located on the desk. The switches are plugged into Kailh hot-swap sockets on the PCB, which is floating and attached only to the sockets.

The floating is fine, but the problems starts with the encoders, which are only connected to the PCB. This means that any pressure on an encoder moves the switches in the sockets. 

From time to time and after transport, I had to rearrange the switches in the sockets.


## Pteron 56
* https://github.com/FSund/pteron-keyboard
* Gateron Silent Brown

## Dactyl / Scylla
{{< refphotos photo="kb_scylla"  opts="250x" >}} 

* https://bastardkb.com/scylla
* Gazzew Boba U4 Silent Tactile Switch 62g


## Cocofly
{{< refphotos photo="kb_chocofly"  opts="250x" >}} 
* https://github.com/vlkv/chocofly
* white chocs
* JLPCB 
* EVQ WGD0001 barrel encoder  (aliexpress only)

## Dactyl monoblock
* https://github.com/joshreve/dactyl-keyboard/pull/79
<!--  ![](monoblock.png)  -->

text davor
{{< imageresize file="monoblock.png" opts="300x200" alt="Monoblock in OpenSCAD" >}}

<!--  {{/*  < imageresize file="/photos/chicago-us/chicago-us.jpg" opts="366x200"  >  */}} --> 


und es geht weiter