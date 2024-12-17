---
layout: page-fullwidth
subheadline: Firmware 
title:  "Slave firmware for Interconnect IO Board"
teaser: "Firmware information of the slave devices used on the interconnect IO Board of the First TestStation"
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
    title: Pico_slave.jpg
    caption: Pico Slave location
    caption_url: https://github.com/dlock8/InterconnectIO_Slave
    author: dlock8
---

## Features
•	The Pico slave firmware acts as the I2C slave controller for the Interconnect IO Box. The Pico slave receives 2 bytes of information (command + parameters) from the Master Pico, processes the command, and returns an answer if necessary.<br>
•	The Pico slave devices are used to perform only basic GPIO actions, which do not require speed.<br>
•	Commands supported by the Pico slave firmware are listed in the GitHub repository InterconnectIO_Slave. For details, refer to the <a href= "https://github.com/dlock8/InterconnectIO_Slave/blob/main/README.md">readme.md</a><br>
•	The I2C addresses used to communicate with the Pico slaves are defined by two hardware lines connected to ground (0) or left open (1).  
•	The slave firmware needs to be loaded onto the three Pico controllers and installed at the location marked in the picture above. <br>


## Flowchart

•	The flowchart below illustrates the algorithm used to process commands received from the Master Pico on the I2C port.<br>

<figure>
  <img src="../../images/Pico_Slave_flowchart.jpg" alt="Slave Flowchart">
  <figcaption>Slave Firmware Flowchart</figcaption>
</figure>

{: .t60 }

{% include list-posts tag='software' %}
