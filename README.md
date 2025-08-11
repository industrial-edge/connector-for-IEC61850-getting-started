# Connector for IEC 61850

This example shows how to use the Industrial Edge app Connector for IEC 61850.

- [Connector for IEC 61850](#connector-for-iec-61850)
  - [Description](#description)
    - [Overview](#overview)
    - [General task](#general-task)
  - [Requirements](#requirements)
    - [Prerequisites](#prerequisites)
    - [Used components](#used-components)
  - [Configuration](#configuration)
  - [Usage](#usage)
  - [Documentation](#documentation)
  - [Contribution](#contribution)
  - [Licence and Legal Information](#licence-and-legal-information)

## Description

### Overview

This tutorial shows how to use the Industrial Edge application Connector for IEC 61850 to establish a connection between an Industrial Edge Device (IED) and Intelligent Electronic Devices (IEDs) in power distribution systems.

The Connector for IEC 61850 is an application that runs on the individual Industrial Edge Device. It provides the functionality to connect to IEC 61850 servers (typically IEDs like protection relays, bay controllers, or merging units) and acquire data. It supports the IEC 61850 standard, which defines communication protocols for electrical substations, utilizing MMS (Manufacturing Message Specification) for data exchange. Connections can be configured using the Common Configurator for Industrial Edge. The connector transfers selected data points from IEC 61850 devices to the Databus. From there, the data can be used within other Edge apps for monitoring, analysis, or integration into higher-level systems.

### General task

In this example, we outline the process of configuring a connection between an Industrial Edge Device (IED) and an IEC 61850 compliant Intelligent Electronic Device (e.g., a Siemens SIPROTEC protection relay) acting as an IEC 61850 server. The Industrial Edge Device, running the Connector for IEC 61850, acts as a client, acquiring real-time measurement values (e.g., current, voltage, frequency) and status information (e.g., breaker status, alarm signals) from the substation IED. This data is then published to the Industrial Edge Databus, making it available for applications like Energy Manager, IIH Essentials, or custom analytics solutions.

## Requirements

### Prerequisites

- Access to an Industrial Edge Management (IEM) with onboarded Industrial Edge Device (IED).
- IEM: Installed System Configurator for Databus.
- IED: Installed apps Connector for IEC 61850, Common Configurator, IIH Essentials, Databus (optional).
- IED (Industrial Edge Device) is connected via network to the IEC 61850 Intelligent Electronic Device (e.g., protection relay).
- An IEC 61850 compliant Intelligent Electronic Device (IED) with an accessible IEC 61850 server interface. In this guide a simulator is being used.

### Used components

- Industrial Edge Management virtual V 2.4.2-3
- Industrial Edge Device 227E V 3.0.0 
  - Connector for IEC 61850 v1.0.0
  - Common Configurator v2.0.1
  - Databus v3.2.1
  - IIH Essentials v2.0.1
  - IIH Semantics v2.0.1 
## Configuration

You can find further information about the following steps in the [Configuration](/docs/Installation.md) documentation:

- [Overview](#overview)
- [Prerequisites](#prerequisites)
- [Used Components](#used-components)
- [IEC 61850 Server (IED/Simulator) Preparation](#iec-61850-server-simulator-preparation)
- [App Installation](#app-installation)
- [Connector for IEC 61850 Configuration](#connector-for-iec-61850-configuration)
- [Data Management](#data-management)
- [Extra: Visualization with Energy Manager](#extra-energy-manager---visualization)

## Usage

Detailed instructions on how to use the Connector for IEC 61850, including monitoring data flow and integrating with other Industrial Edge applications, can be found in the [Usage](/docs/Usage.md) documentation.

## Documentation

You can find further documentation and help in the following links:

*   [Siemens Industrial Operations X Documentation](https://docs.industrial-operations-x.siemens.cloud/)
*   [Connector for IEC 61850 Overview](https://docs.industrial-operations-x.siemens.cloud/r/en-us/v2.0.0/connector-for-iec-61850/overview/introduction-to-connector-for-iec-61850)
*   [Industrial Edge Hub](https://iehub.eu1.edge.siemens.cloud/#/documentation)
*   [Industrial Edge Forum](https://www.siemens.com/industrial-edge-forum)
*   [Industrial Edge landing page](https://new.siemens.com/global/en/products/automation/topic-areas/industrial-edge/simatic-edge.html)
*   [Industrial Edge GitHub page](https://github.com/industrial-edge)
*   [IEC 61850 Standard (External Resource)](https://www.iec.ch/iec-61850)

## Contribution

Thank you for your interest in contributing. Anybody is free to report bugs, unclear documentation, and other problems regarding this repository in the Issues section.
Additionally, everybody is free to propose any changes to this repository using Pull Requests.

If you haven't previously signed the [Siemens Contributor License Agreement](https://cla-assistant.io/industrial-edge/) (CLA), the system will automatically prompt you to do so when you submit your Pull Request. This can be conveniently done through the CLA Assistant's online platform. Once the CLA is signed, your Pull Request will automatically be cleared and made ready for merging if all other test stages succeed.

## Licence and Legal Information

Please read the [Legal information](LICENSE.md).