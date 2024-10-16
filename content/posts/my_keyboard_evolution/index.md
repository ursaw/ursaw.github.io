+++
title = "My Keyboard Evolution"
date = 2022-08-29
tags = ['keyboards']
+++


## TL;DR
This is my historically ordered journey into ergonomic keyboards. I try to explain the background of each choice, the advantages and limitations.

My main work on computers is coding, and I like terminals/consoles and try avoid using the mouse as much as possible.

From IBM model M to Dactyl split ortho keyboard for ergonomics and fun. I am still use QWERTY, but try slowly  to move to [COLMAK DH](https://colemakmods.github.io/mod-dh/keyboards.html#matrix-keyboards) with the [tarmac transition](https://forum.colemak.com/topic/1858-learn-colemak-in-steps-with-the-tarmak-layouts/).

It was an evolution with many small changes, today I advise a quick jump to a split ortho keyboard or mono blocks.



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



### Happy Hacking Keyboard lite 2

I have tried the [HHKB Lite 2](https://deskthority.net/wiki/HHKB_Lite) only very briefly. I like the [HHKB layout](http://web.archive.org/web/20021006065050/http://www.pfuca.com/products/hhkb/litelayout.html) variant on the top right, the backspace key in row 2 and two 1U keys instead of the 2U backspace key and the small cursor keys. For me, it was the first time I had a very useful internal USB hub.

I didn't have a chance to get familiar with the Sun Type 3 keypad. I was never able to press the control key properly.

But I really didn't like typing on it because of the tying angle and the heavy rubber dome switches. 

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

For my second built I dared a more complex build, and it take a while for me to get used to solder SMD diods. I already summarized my [first impression](/posts/thoughts_soflev1) of the Sofle, and this is the keyboard I have used most often (besides the [model M](#ibm-model-m)) and therefore its like a reference for me.

Most of the following builds are like 4x6+4 boards to me, as I can't live so far with fewer keys.

### Design Error
The Sofle has a small design flaw for which I have no solution. 

If you follow the key press, you hit the switch, which is mounted in the switch plate. The plate is connected with stand-offs to the back plate, which is located on the desk. The switches are plugged into Kailh hot-swap sockets on the PCB, which is floating and attached only to the sockets.

The floating is fine, but the problems starts with the encoders, which are only connected to the PCB. This means that any pressure on an encoder moves the switches in the sockets. 

From time to time and after transport, I had to rearrange the switches in the sockets.


## Pteron 56


{{< refphotos photo="kb_Pteron56"  opts="250x" >}} 


* https://github.com/FSund/pteron-keyboard
* Gateron Silent Brown

After realizing the travel limitations of the Sofle, I decided to go with the [Pteron 56](https://github.com/FSund/pteron-keyboard). This was my first [handwired](https://github.com/qmk/qmk_firmware/blob/master/docs/hand_wire.md) keyboard that I built, but it was easier than I expected. The only build instruction I was using was having a quite thoroughly look at the picture [builds\Pteron56_ wiring.jpg](https://github.com/FSund/pteron-keyboard/blob/master/builds/Pteron56_%20wiring.jpg) and the QMK files.

I came across a few drawbacks of the Pteron, and that's why you'll find more keyboards in this list...

- First of all, I can't recommend Gateron Silent Browns, although I like to standard Gateron Browns. Sure they are quiet, but after using them I realized what people mean when they talk about scratchy switches.

- The thumb cluster is far is much too inward for me. When I tried to reach the innermost keys with my thumbs, I had to travel with my whole hand. This never happened with the reference Sofle.

- The height of the keyboard is too much for me. I could reduce it with smaller distance screws. But in any case I would need a wrist rest (is a wrist rest ergonomic at all?) to keep my hands from bending too much.

## Dactyl / Scylla
{{< refphotos photo="kb_scylla"  opts="250x" >}} 

* https://bastardkb.com/scylla
* Gazzew Boba U4 Silent Tactile Switch 62g

So far I've only built planar keyboards, but I've always been interested in concave designs of dactyls, which is nicely illustrated in the great [adereth dactyl video](https://www.youtube.com/watch?v=uk3A41U0iO4).

It took me a while to get around to buying a kit from [bastardkb](https://bastardkb.com/scylla), because for a long time I was too cheap to do so. The kit and building instructions from bastardkb are great, and it was easy to complete the build, and not just for me, after all my building experience.

I opt for Boba Tactil, which are unexciting switches. Personally, I prefer a more pronounced tactility like Zealios, but they are OK. 

The Scylla offers a nice typing experience, although it took me a while to get fully used to it. From time to time, I painfully realize that I'm using the wrong finger for a column, which would be lost on a planar keyboard.

The tenting angle could be a little higher, so I had Treatstock print out the [30 degree tenting angle](https://github.com/Bastardkb/Scylla/tree/main/files). But that is then too much for me. Additionally you need a desk mate, because otherwise the halves start to move. As you can see in the picture, I like to have a trackball in the middle, which is not possible with the high tenting.

## Chocofly
{{< refphotos photo="kb_chocofly"  opts="250x" >}} 

* https://github.com/vlkv/chocofly
* white chocs
* JLPCB 
* EVQ WGD0001 barrel encoder (aliexpress only)

Right after I discovered [Chocofly](https://github.com/vlkv/chocofly), I made the decision to build it to come accross the disadvantages of the Pteron 56.Switching to chocs was a new adventure because I had to purchase new switches as well as keycaps. I discovered white chocs, which I really like. Afterwards I also got Kailh MX white for my Sofle, but I like prefere the chocs.

The height of the keyboard, which is just a circuit board and the switches, is perfect. I mainly place the Chocofly directly on the laptop's internal keyboard in the Sonshi Style and it works really well.

I ordered the PCB from JLCPCB the barrel encoder from Aliexpress, which means waiting again. 


Although I like the rotary encoder on the Sofle for page up and down, I rarely use the barrel encoder, maybe it's on the wrong hand, or maybe it's too far away. 

As you can see in the picture, I don't even need all the thumb keys because they are too far inside for me.  




## Dactyl monoblock

{{< refphotos photo="kb_Dactyl_monoblock"  opts="250x" >}} 

* https://github.com/joshreve/dactyl-keyboard/pull/79, and [pull req. 85](https://github.com/joshreve/dactyl-keyboard/pull/85)
* Treatstock printout
* both Gateron brown
* 2nd iteration with rotary encode (page up/down and sound)

Based on the [python dactyl](https://github.com/joshreve/dactyl-keyboard/) code I added a design parameter __monoblock__ with two iterations so far. The second version has room for an trackball.

Since for cost reasons I used a pro micro for both versions, I had to use a 8x8 matrix for the rotary encoder version instead of a simple 12x5 matrix. Soldering the 8x8 matrix makes more work and trouble than I thought in advance. Unfortunately, it was only after the fact that I found a way to enable more pins at https://golem.hu/guide/pro-micro-upgrade.

I use it in the office, but since I use a Scylla at home, I am always confused with the thumb cluster.

Therefore I have to go on...

## Dactyl / Charybdis
{{< refphotos photo="kb_charybdis"  opts="250x" >}} 
* https://bastardkb.com/charybdis/
* Kailh tactil white
* Matt3o MT3 /dev/tty keycaps
* ~~[Amoeba king royals](https://github.com/mtl/keyboard-pcbs)~~ hand wired

Before going the step to my long planned dactyl monoblock with a trackball I decided to take a very small evolution step and build a [bastard Charybdis](https://bastardkb.com/charybdis/). 
Initially I was going for [Amoeba king royals](https://github.com/mtl/keyboard-pcbs) to have the ability to change switched with Kailh hot swap sockets, but this turned out not to be the best idea. 
When I wanted to place the soldered PCBs in the case, I realized that they don't really fit well, and it would be a hazel to exchange the switches. Setting up the PCBs is a very long and tedious work and in my opinion it only make sense to use them, when additionally set up LEDS (SK6812 mini). Therefore, I just soldered the white Kailh into the cases. 

I was really curious about the 34mm trackball. But in the end I am a little disappointed, because it is not working well for me with thumb.

## IK
{{< refphotos photo="kb_ik"  opts="250x" >}} 
* https://github.com/ianmaclarty/ik
* [Gateron Low Profile KS-33](https://ergonautkb.com/docs/switches/gateron-low-profile/) brown
* XVX key caps

I was very curious about the Gateron Low Profile switches, and also considered to build an [Ergonaut One](https://ergonautkb.com/docs/keyboards/ergonaut-one/intro/), but i hesitated to get rid of the number row. 

In the end I am very impressed about the reduced height of the IK, this reminds me to the Chocofly. The default GLP browns are quite OK, initially I planed to have my first board with red switches. I build one wit reds and one with browns, but was very disappointed of the reds. 

Its a great travel board, could be seen as a  [voyager](https://www.zsa.io/voyager) clone. Recently, I had the chance to get a voyager in my hands, and teher is no  denying that the voyager has an outstanding quality!

## Chrumm 
{{< refphotos photo="kb_chrumm"  opts="250x" >}} 
* https://github.com/sevmeyer/chrumm-keyboard
* brown switches
* OEM key caps
* JLCPCB print

I inserted this build to get my family into ergonomics. They rely on German key layout. The chrumm offers an interesting asymmetrical layout, which gives room for all special keys. The concept and the entire prepared files are of a very high quality, which make its worth to build this board.

This was my first board where I was surprised of the sound, usually this is not an topic for me, but the board is quite solid and offers an nice typing feeling, inclusive an descent sound.  



## Upcoming trackball monoblock

<!---
![](monoblock_trackball.png)
--->


{{< imageresize file="monoblock_trackball.png"  opts="300x200"  alt="Monoblock in OpenSCAD" >}} 


My next keyboard will be a Dactyl monoblock with a center trackball, which will be something like the [Charybdis](https://bastardkb.com/charybdis/) with an [internal trackball (github)](https://github.com/ursaw/dactyl-keyboard/tree/monoblock_center_trackball).

I got confused with the mini thumbc luster on the Dactyl monoblock and the thumbcluster with 5 keys on the Scylla. Therefore I go with the __MINI__ 5-key thumb cluster now.

I have already sourced all the parts and am looking for a window of time to build it. Unfortunately, in the meantime, I have more ideas that I will incorporate into the next monoblock. Optionally I will go with an STM32F103C8T Blue Pill based and may add an internal USB port.


But will this really be my endgame?

I will update.
