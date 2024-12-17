---
layout: page-fullwidth
subheadline: Printed Circuit Board
title:  "Interconnect IO Board PCB"
teaser: "Routing of the Interconnect IO Printed Circuit Board (PCB)"
meta_teaser: ""
breadcrumb: true
categories:
    - hardware
tags:
    - blog
    - content
    - post
    - post format
image:
    title: IOBoard_pcb.png
    caption: Interconnect IO Board source file
    caption_url: https://github.com/dlock8/InterconnectIO_Board
author: dlock8
---

## Features

•	 Design of the Interconnect IO board was carried out using the open source software Kicad V7.x. <br>
•	 Inteconnect Io board source files are available on Github. Link: <a href= "https://github.com/dlock8/InterconnectIO_Board">InterconnectIO_Board</a><br>
•	 For mode details, please refer to the electrical schematic.<br>
•	 On board, hundred of Net Tie components (NTxxx) have been installed to help with on-board modification. The NetTie PCB component facilitates modification routing by providing a clear space where PCB traces can be cut (cut between two holes) and changed routing by adding wire (solder on one of the holes on each side of the trace cut).<br>
•	 Board users can either use already developed specialized modules available on the market at a low cost, or solder surface-mount components directly onto the board to achieve the same functionality.<br>
•	 The Pico Board can be soldered directly on the board, but I recommend mounting it on a female socket so that it can be easily replaced.<br>
•	 In the picture above, only through-hole components are soldered on the PCB. Using piggyback connectors, the specialized module will be mounted on the female sockets.<br>
•	Low-power Relays, integrated circuits, and transistors are recommended to be mounted on sockets to allow for easy replacement.
•	For serial interfaces (close to power switches), two different types of modules are available with two different voltages (5V and 3.3V). The voltage will be selected using a female jumper. It is best to use 3.3V, but Pico modules are capable of working at 5V as well.<br>
•	The protection fuse is mounted in a socket to make replacement easy.<br>
•	There is a reserved area for a custom module that will be added in the future<br>
•	The PCB has two soldered screw holders on each side of the 96-pin connector. The purpose of these components is to precisely attach the external mechanical PCB rail to the PCB.<br>
•	This board is protected against reverse voltage and high voltage with a 5.5V protection diode (fuse will burn if high voltage is applied).<br>


{: .t60 }

{% include list-posts tag='hardware' %}



