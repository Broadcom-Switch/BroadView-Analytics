
Overview
========
This document describes how to use the Broadcom(C) BroadView(TM) Analytics application which provides the ability to visually manage and monitor various switches using the following features:
   - Monitoring on-chip buffers (Buffer Statistics).
   - Monitoring congestion drop counters.
   - Tracing packets across a Link Aggregation Group (LAG) and an Equal-Cost Multipath (ECMP) group (Packet Trace).
   - Deep visibility into various flows passing through the Switch using Flow Tracker.

This document is intended for software users with a good knowledge of networking and BroadView-related features.

The BroadView Analytics application works with the BroadView Instrumentation Agent for device management and to manage individual BroadView features supported by the switch. The application provides an easy-to-use Graphical User Interface (GUI) and enables user to view advanced analytics and troubleshoot network issues. Key features supported by the software are:

 - Leveraging the unique silicon instrumentation capabilities supported by the StrataXGS(R) BCM56760, BCM56850, BCM56860, BCM56870, BCM56960 and BCM56965 silicon families.
 - Threshold-based monitoring, buffer statistics tracking, and triggers for proactive monitoring and scalability.
 - Congestion drop counters in the ASIC.
 - Aggregating group resolution to ensure optimal utilization of group members and avoid hash polarization.
 - Deep visibility into the flows passing through the Switch.

System Requirements
===================
The BroadView Analytics application runs in a Java Virtual Machine (JVM). Being a Java application, it can potentially run on any operating system that supports Java. However for best results, Broadcom recommends using the application on Microsoft Windows 10 and above. Before user execute the application, ensure that the computer meets the minimum requirements listed below.

|**System Requirements**|**Description**|
-------------------|------------
|Operating System| Microsoft Windows 10 and above|
|Memory| 4 GB|
|Free Hard Disk Space| at least 3 GB|
|Java Virtual Machine (JVM)|Java version 1.8 and above|
|Hardware/System Verification Kit (SVK)|BCM56760, BCM56850, BCM56860, BCM56870, BCM56960 and BCM56965 silicon families|
|Traffic Generator and Connectors|Traffic Generator to send traffic|
|BroadView Agent Software Version|3.2.0.2|

Supported ASIC Families
===================
|**Feature**|**ASIC Family**|
-----------|---------
|Monitoring On-Chip Buffers|BCM56760, BCM56850, BCM56860, BCM56870, BCM56960 and BCM56965|
|Tracing Packets across a LAG or ECMP Group|BCM56870, BCM56960 and BCM56965|
|Flow Tracker|BCM56870|

Quick Start
===========
To quickly begin with the BroadView Analytics application, use the following steps.

1. Launch the BroadView Analytics application
    - Clone the repository: **git clone https://github.com/Broadcom-Switch/BroadView-Analytics.git**
    - Navigate to **BroadView-Analytics/bin**
    - Execute: **java -jar broadview-analytics.jar** from command line
    - Note that the default report receiving server port is **9070**
2. Start the BroadView Instrumentation Agent on the  switch
    - Make sure to have Switches with BCM56760, BCM56850, BCM56860, BCM56870, BCM56960 or BCM56965 families.
    - Run the BroadView Instrumentation Agent on the switch.
    - Make sure that the default reporting client port is set to **9070** (or the port number is configured as in the report receiving server in the previous step) and the default TCP port number is **8080** (used to communicate with the BroadView Analytics application).
3. Switch auto-registration
    - BroadView Agent supports auto-registration messages, the switch is automatically registered and displayed in the BroadView Analytics User Interface
4. Make sure to have the necessary infrastructure to generate the traffic on the ports to perform instrumentation operations

Supported Features
==================
 - [Switch Registration](REGISTRATION.md)
 - [Monitoring On-Chip Buffers](BST.md)
 - [Tracing Packets across a LAG or ECMP Group](PT.md)
 - [Flow Tracker](FT.md)

