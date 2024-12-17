---
layout: page-fullwidth
subheadline: Block Diagram
title:  "SelfTest Board Block Diagram"
teaser: "Selftest Board contains electronics and routing required to validate the ressources contains on the First TestStation"
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
    title: Selftest_bd.png
    caption: 
    caption_url: 
author: dlock8
---

## Features

•	 The Selftest will be able to verify the Interconnect IO Board without the use of external instruments. A better precision could be achieved, however, if external instruments are connected for verification. <br>
•	The test strategy uses relays to multiplex the different power sources (PS1 - PS10). We use the same strategy to measure the results (VM1 - VM6).<br>
•	 As part of the test strategy, stimulus will be applied to PS1 and voltage will be observed on VM1 to validate basic function. We will validate the digital port in seconds in order to make sure the selftest board relays are working as they should.<br>
•	 The strategy for testing relay contacts is based on current measurement.  A power source is applied to one side of the relay contact, while the other side is grounded.<br>
•	 Current and voltage are measured to determine if the relay's contact resistance is within the limit. It is possible to measure current using either the IN219 module or the DMM (Amp input). The circuit has been designed to limit the maximum current by adding a low value resistance.<br>
•	 There is a provision on the selftest board to validate the 4-wire resistance measurement if an external DMM is present.<br>
•	 To avoid overloading the Pico ADC (3V limit), we divide the voltage applied to ADC0-ADC1 by 2.<br>
•	 Transistors with open collectors are used to toggle relays, and are validated by measuring voltage at their collectors when active (0V) and inactive (5V).<br>
•	 The validation of digital ports is performed by connecting signals by pair, configuring one line as input and the other as output, applying stimulus at the output, and reading the response at the input.<br>
•	 Relays present on the selftest board can also be activated using digital ports.<br>
•	 The relay bank is connected to each other so that it can be tested simultaneously. The test will identify the defective line, but will not determine which relay needs to be replaced (choice of two).<br>
•	 External instrument other than power supply and DMM will be tested by connecting stimulus instrument (ex: AWG) to the oscilloscope input.<br>
•	 Using a Pico module, digital communication will be tested. All communication protocols will be validated by the firmware on Pico.<br>
•	 Besides digital ports, the Pico module can also validate basic digital signals.<br>
•	 The purpose of a 1-wire device is to be able to read information about UUTs (which board is connected?). The board is equipped with two 1-wire devices, one for each connector if a mating cable is used instead of a single board.<br>
•	 The high speed device is connected via two connectors (USB and Ethernet). The plan is to connect the flash drive on USB and loopback on Ethernet.<br>
•	 Space for custom module is present on Selftest Board.<br>


{: .t60 }

{% include list-posts tag='design' %}




