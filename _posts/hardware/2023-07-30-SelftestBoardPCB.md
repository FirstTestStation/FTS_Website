---
layout: page-fullwidth
subheadline: Printed Circuit Board
title:  "Selftest Board PCB"
teaser: "Routing of the Selftest Printed Circuit Board (PCB) used to validate First TestStation"
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
    title: Selftest_pcb.png
    caption: Selftest Board source file
    caption_url: https://github.com/dlock8/Selftest_Board
author: dlock8
---
## Features

•	 Design of the Selftest board was carried out using the open source software Kicad V7.x. <br>
•	 Selftest board source files are available on Github. Link: <a href= "https://github.com/dlock8/Selftest_Board">Selftest_Board</a><br>
•	 For mode details, please refer to the electrical schematic on Github.<br>
•	 On board, hundred of Net Tie components (NTxxx) have been installed to help with on-board modification. The NetTie PCB component facilitates modification routing by providing a clear space where PCB traces can be cut (cut between two holes) and changed routing by adding wire (solder on one of the holes on each side of the trace cut).<br>
•	 Active components are mounted on sockets to facilitate replacement.<br>
•	 There is a reserved area for a custom module that will be added in the future.<br>

{: .t60 }

{% include list-posts tag='hardware' %}
