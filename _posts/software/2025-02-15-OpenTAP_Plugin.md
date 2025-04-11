---
layout: page-fullwidth
subheadline: software
title:  "OpenTAP Plugin of InterconnectIO Box"
teaser: "Integrate and automate your testing process with the OpenTAP Plugin for the InterconnectIO Box on the First TestStation!"
meta_teaser: ""
breadcrumb: true
categories:
    - software
tags:
    - blog
    - content
    - post
    - post format
image:
    title: TAP_plugin.jpg
    thumb: TAP_plugin.jpg

---

---

## Purpose

The **InterconnectIO Box** has been developed to support communication using the **SCPI** protocol. However, building test sequences solely with raw SCPI commands can quickly become tedious and time-consuming. By leveraging our chosen test sequencer, **OpenTAP**, we can create more efficient and maintainable methods to interact with the instrument.

One of OpenTAP’s key features is the concept of **Test Steps** — small programs written in **C#** or **Python** that perform either a basic or advanced operation:

- A **basic Test Step** might simply send a `*IDN?` command to the instrument and return the response.
- An **advanced Test Step** could send the same command, analyze the response, and assign a verdict (e.g., **PASS** or **FAIL**) based on predefined criteria.

All the necessary Test Steps for communicating with the selected instruments (InterconnectIO Box) are grouped together and packaged into what OpenTAP calls a **Plugin**.

In essence, the plugin transforms the InterconnectIO Box from standalone hardware into a fully integrated, intelligent component of your test workflow — greatly enhancing its usability and performance.

If you’re interested in exploring further, visit the [OpenTAP documentation](https://doc.opentap.io/) for in-depth information on plugin development and usage.

## InterconnectIO Box Plugin

As shown in the image above, the actual plugin for the **InterconnectIO Box** includes the following components, all integrated within the same plugin package:

1. **InterconnectIO Plugin**  
   This plugin groups together all the Test Steps required to execute the full range of functions available on the InterconnectIO Box.

2. **DUT Plugin**  
   This plugin defines the **Device Under Test (DUT)**. According to our DUT strategy, each DUT should include a 1-Wire device, which is read and validated before power is applied. This plugin is responsible for defining the expected 1-Wire data to be validated during the test sequence.

3. **Selftest Board Plugin**  
   This plugin provides communication with the **Selftest Board**, and is developed as an integrated part of the InterconnectIO Box Plugin. While it's not required when the DUT is not a Selftest Board, it adds powerful and maintainable Test Steps for internal diagnostics and validation.


## Plugin Description

All the Test Steps required to control the **FTS_InterconnectIO Box** have been organized into distinct categories for better clarity and ease of use:

- **1-Wire**  
  A set of Test Steps to check, read, or write data from 1-Wire devices.

- **Analog**  
  Test Steps to read voltages from the ADC, set voltages using the DAC, take measurements from the Power Monitor, control individual relays, and toggle open-collector transistors.

- **Communication**  
  Test Steps to configure and perform read/write operations using communication protocols such as **I2C**, **SPI**, and **Serial**.

- **Config**  
  Test Steps to read from or write to configuration parameters stored in the configuration EEPROM.

- **Digital**  
  Test Steps to configure direction (**Input/Output**) and perform bit- or byte-level read/write operations on one of the two 8-bit I/O ports.

- **GPIO**  
  Test Steps to set the direction of individual GPIO pins and perform read/write operations on designated GPIOs.

- **Route**  
  Test Steps to control one of the four available relay banks.

- **SCPI**  
  Test Steps to send predefined basic SCPI commands or manually send/query SCPI instructions.

- **System**  
  Test Steps to monitor and control system-level features, including reading firmware and software version details.

- **ZModule**  
  Test Steps dedicated to controlling the **Selftest Board**, enabling seamless command and response communication between the box and the Selftest module.

## Plugin Location

The plugin source code is hosted on the official GitHub repository. In the future, the **InterconnectIO Box** plugin may also be made available directly through the **OpenTAP Package Manager** for easier installation and updates.

🔗 [OpenTAP InterconnectIO Box Plugin](https://github.com/FirstTestStation/FTS_InterconnectIOBox_OpenTAP_Plugin)



{: .t60 }

{% include list-posts tag='software' %}
