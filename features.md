---
layout: page
title: Features
permalink: /features/
---

<div class="row"> 
<div class="col-sm-4">
 <div class="panel panel-primary">
   <div class="panel-heading">
     <h3 class="panel-title">My knitting, my pattern!</h3>
   </div>
   <div class="panel-body">
   Pixels are needles, needles are pixels. Getting from an image on your computer to a cosy sweater in a very simple and convenient manner. Thus you can decide what you want to wear!
   </div>
 </div>
</div>

<div class="col-sm-4">
 <div class="panel panel-primary">
   <div class="panel-heading">
     <h3 class="panel-title">Go Big!</h3>
   </div>
   <div class="panel-body">
   AYAB supports the whole width of the Brother knitting machines, which are 200 needles (also called pixels) wide. Even better: Your image can have an infinite number of height lines or rows. You can knit and knit and knit and knit...!
   </div>
 </div>
</div>

<div class="col-sm-4">
 <div class="panel panel-primary">
   <div class="panel-heading">
     <h3 class="panel-title">Easily applicable</h3>
   </div>
   <div class="panel-body">
   The AYAB hack (as we call our Arduino and shield) is non-destructive and fully reversible! That is, if you want to go back to the original Brother technology again (I bet you won't), simply remove the AYAB hardware, reconnect the Brother controller and everything is back to its original state, just like in the 1970's! 
   </div>
 </div>
</div>
</div> <!-- row -->

<div class="row"> 
<div class="col-sm-4">
 <div class="panel panel-primary">
   <div class="panel-heading">
     <h3 class="panel-title">Ribber Extension</h3>
   </div>
   <div class="panel-body">
   Luckily for you, the AYAB Hack also supports the Ribber Extension for Brother Knitting Machines. 
   </div>
 </div>
</div>

<div class="col-sm-4">
 <div class="panel panel-primary">
   <div class="panel-heading">
     <h3 class="panel-title">4- and 6-Colour Knitting</h3>
   </div>
   <div class="panel-body">
   Rainbowlicious! 
   For the lucky owners of a 4- or 6- colour changer: AYAB will soon be supporting knitting with more than 2 colours!
   </div>
 </div>
</div>
</div> <!-- row -->

<div class="row"> 
    <div class="col-sm-6">
<p>The goal of the AYAB project is to provide an alternative way to control the famous Brother KH-9xx range of knitting machines, e.g. KH-910 and KH-930.</p>

<p>There are some similar projects on the internet, such as Knitic or, of course, ladyada's electro-knit.</p>

<p>The main drawback behind the existing projects is that they make use of the 930/40 series of knitting machines - which are still pretty expensive in a good working condition and they must be in a working condition!<br>
The AYAB uses the older KH-910 model, which is far cheaper than the other models, mainly because it features an error-prone scanner mechanism for reading the image data (but we don't care because we don't use the scanner anyway, nor the computer part either…).<br>
The 930/940 series already use some kind of digital programming, which opens even more ways to hack them, other than the way this project does it. But that is not necessarily better than AYAB does it!!</p>

<p>Normally, the KH-910 is programmed using semi-transparent picture cards which are scanned by the machine line by line. Using this information, the machine sets the needles accordingly to achieve the knitting of the picture shown on the picture card.<br>
Probably due to memory restrictions (the machines are quite old today), the machine only supports pictures with a max of 60 needles (= pixels) width, although the machine has a total width of 200 needles. But at least, it is possible to “copy and paste” the scanned image multiple times to achieve a banner-like usage of the scanned data (useful for Norwegian patterns).</p>

</div>

<div class="col-sm-6"> 
<p>With the AYAB interface, you can supply the knitting machine with a digital image from your computer using simple software such as Paint or GIMP, under most windows and some Linux variants. Thus the restriction of a 60 pixel/needle image width has also simply been abolished due to the vastly improved control that AYAB interface has over the original Brother design. You can now just simply knit an image with up to a 200 needle/pixel width.</p>
               
<p>The control of the needles and the needed identification of the current position and direction of movement of the knitting carriage are supplied by a cheap and well-known Arduino microcontroller, combined with a custom developed shield (the name for an “interface” in the Arduino world) for the knitting machine.<br>
You actually only need to open up one part of your knitting machine (warranty is void anyway for some years now…) and simply replace the existing control board (the one with all the switches and LEDs on it) with the AYAB controller, then link the Arduino part of this interface (shield) with your computer and start knitting!<br>
(Well almost! This does assume that the power supply and needle solenoids of your Knitting Machine [called a KM from now on!!] are all in a good working order!)</p>

<p>The API (Application Programming Interface ) to the Arduino is designed in a simple and straight forward manner, so that the control of the machine can be taken over by almost every piece of knitting machine software which can access the USB port of your computer (or raspberry pi, or …).<br>
The API consists only of three commands (request information about the controller firmware, request the start of a new picture, send line[x] to the controller when the controller requests it).</p>

</div>
</div> <!-- col-sm-12 -->

