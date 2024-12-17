---
layout: page-fullwidth
subheadline: Firmware 
title:  "Master firmware for Interconnect IO Board"
teaser: "Firmware information of the master device used on the interconnect IO Board of the First TestStation"
meta_teaser: ""
breadcrumb: true
categories:
    - firmware
tags:
    - blog
    - content
    - post
    - post format
image:
    title: Pico_master.jpg
    caption: Pico Master location
    caption_url: https://github.com/dlock8/InterconnectIO_Master
    author: dlock8
---

## Features

•	The Pico master firmware is the main controller of the interconnect IO Box.  The Master receive SCPI command from serial port, execute the command and return the answer. <br>
•	The Pico Master device is used to control the Interconnect IO Board and handle the communication protocols available on the board (I2C, SPI, Serial, and 1-Wire).  <br>
•	SCPI commands supported by the Pico master firmware are listed in the GitHub repository InterconnectIO_Master. For details, refer to the <a href= "https://github.com/dlock8/InterconnectIO_Master/blob/main/README.md">readme.md</a><br>
•	Thanks to the open-source SCPI device library written by Jan Breuer, available at  <a href= "https://www.jaybee.cz/scpi-parser/">SCPI parser</a><br>
•	Detailed messages to aid in debugging or understanding the process flow are available through the USB connector of the Pico controller.<br>
•	The configuration EEPROM is used to store user preferences.<br>
•	On error, the 'Red Fail' LED on the front panel will turn ON, and a beep will sound for a short duration.<br>
•	The Master firmware needs to be loaded onto the Pico controller and installed at the location marked in the picture above. <br>


## Flowchart

•	The flowchart below illustrates the algorithm used to process SCPI commands received on the serial port.<br>

<figure>
  <img src="../../images/Pico_Master_flowchart.jpg" alt="Master Flowchart">
  <figcaption>Master Firmware Flowchart</figcaption>
</figure>

{: .t60 }

{% include list-posts tag='software' %}
