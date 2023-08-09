---
layout: page-fullwidth
subheadline: Printed Circuit Board
title:  "Selftest Board PCB"
teaser: "Routing of the Selftest Printed Circuit Board (PCB) used to validate First TestStation"
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
    title: Selftest_pcb.png
    caption: Selftest Board source file
    caption_url: https://github.com/dlock8/Selftest_Board
author: dlock8
---
## Features

•	 Design of the Interconnect IO board was carried out using the open source software Kicad V7.x. <br>
•	 Inteconnect Io board source files are available on Github. Link: <a href= "https://github.com/dlock8/Selftest_Board">Selftest_Board</a><br>
•	 For mode details, please refer to the electrical schematic.<br>
•	 On board, hundred of Net Tie components (NTxxx) have been installed to help with on-board modification. The NetTie PCB component facilitates modification routing by providing a clear space where PCB traces can be cut (cut between two holes) and changed routing by adding wire (solder on one of the holes on each side of the trace cut).<br>
•	 There is a reserved area for a custom module that will be added in the future.<br>

### All Header-Styles 
{: .t60 }

{% include list-posts tag='design' %}
