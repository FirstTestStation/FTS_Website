---
layout: page-fullwidth
subheadline: Block Diagram
title:  "InteconnectIO Box Block Diagram"
teaser: "InterconnectIO Box is an intelligent hardware interface connected between the UUT and the test equipments."
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
    title: Interconnect.png
    caption: 
    caption_url: 
author: dlock8
---
## Features

•	The InterconnectIO Box is designed to contain most of the electronic components necessary to validate an electronic card or electronic system without the need for additional hardware.<br>
•	SCPI commands will be used over a serial port to communicate with interconnectIO boxes.<br>
•	The InterconnectIO Box can be used to connect electronic instruments directly to the front connector for use by UUTs (Unit Under Tests).<br>
•	The InterconnectIO Box can accept a range of instruments, but most of the resources will be devoted to standard instruments (such as multimeters, oscilloscopes, power supplies, and signal generators) often seen in production test stations.<br>
•	Four relay banks of 8 to 1 are available on the InterconnectIO Box to assist with signal measurement and power distribution.<br> 
•	Each relay bank offers differential (8 to 1) or single ended (16 to 1) routing.<br> 
•	There are two 8-bit bidirectional digital ports available for connection to the UUT.<br>
•	InterconnectIO Box supports the standard low-level communication interfaces used by electronics cards (SPI, I2C, Serial, 1-Wire). The InterconnectIO Box requires external resources to be connected to most complex communication interfaces (USB, JTAG, Ethernet).<br>
•	There are three open collector outputs (30V) available to the UUT.<br>
•	In the Interconnect box, general purpose relays (Low power relays, High power relays, and Solid state relays) are available for free use by UUTs.<br>
•	An InterconnectIO Box has analog resources (ADC, DAC, and Current Sense) used during self-testing. UUT can use these resources for free, but protection is limited.<br>
•	The UUT has access to a lower value power resistor, which will be used as a resistive load to validate the power supply during selftests.<br>
•	EEprom is present on board to save Interconnect Box IO parameter.<br>
•	A custom module can be added to the Interconnect Box IO to contain additional electronics.<br>
•	The CTRL connector has two bidirectional digital IO lines for monitoring and controlling external devices.<br>
•	The InterconnectIO Box requires a 5V@3A power pack to operate effectively. This power supply not only powers the internal components but also provides 5V output to the front connector, which is protected by a fuse for safety.<br>



{: .t60 }

{% include list-posts tag='design' %}






