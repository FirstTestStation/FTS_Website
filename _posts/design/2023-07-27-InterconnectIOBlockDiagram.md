---
layout: page-fullwidth
subheadline: Block Diagram
title:  "Inteconnect IO Board"
teaser: "Inteconnect IO Board contains electronics required to interface with the UUT"
meta_teaser: ""
breadcrumb: true
categories:
    - design
tags:
    - blog
    - content
    - post
    - post format
image:
    title: Interconnect_io_bd.png
    caption: 
    caption_url: 
author: dlock8
---
## Features

•	Interconnect IO Boards are designed to be easy to build and repair.Surface mount components could be soldered directly on board or bought in pre-assembled modules and mounted on Interconnect IO boards through through-hole sockets.<br> 
•	There are many basic components, such as resistors, transistors, relays, leds, etc., which are through-hole component and easy to solder.<br>
•	Old Through-hole technology will be blended with a newly introduced raspberry pi module (Pico) to form a powerful combination of electronics for testing electronics cards or systems.<br>
•	The Raspberry Pico controller was chosen due to its low price, the resources available, and the documentation and programming examples. Four Pico modules were required to provide all the resources needed on the First TestStation project.<br>
•	In order to communicate with each other, Pico modules use an internal I2C bus with a master and three slaves configuration.
•	Communication with external computers is handled by the Master Pico. Low-level communication with UUTs is also handled by Master Pico. A debug port is available on each Pico (master and slave) when a USB cable and interface are connected.<br>
 •	The level shifter device protects the Pico digital pins (limited to 3.3V) and allows testing at higher voltages.<br>
 •	If necessary, synchronization pins (CTRL and FLAG) have been added to work with digital ports.<br>
 •	The Pico ADC inputs will be protected against voltage when the Interconnect IO Board is not powered.<br>
 •	Relay banks use DPDT (Double Pole Double Throw) relays because they are widely available and cheap. The addition of one more relay (COM relay) will allow eight differential relays to be transformed into sixteen single ended relays by reversing the signal.<br>
  •	The board includes a beeper that alerts the user to SCPI communication errors. A front panel error led also indicates error to the operator.<br>
  •	The front panel also includes a power indicator to indicate whether the interconnect IO board is connected to the UUT (Level shifter is enabled and 5V power is available).<br>
 •	A 5V power module is needed to power the Interconnect IO Board. Alternatively, the same 5V power module could be used to power the UUT, but with a limited current (protected fuse).<br>  
•	A voltage of at least 3.3V must be applied to DIG_PWR_IN in order to power the level shifter. There is a voltage level that is defined by the interface of the UUT (normally 3.3V or 5V).  If digital resources are needed, the voltage is mandatory.<br>









