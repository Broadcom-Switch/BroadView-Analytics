
BroadView Analytics
===================
BroadView Analytics Application provides the ability to visually manage and monitor various BroadView features.

Overview
========
BroadView Analytics is a Java based application that provides a GUI based interface to configure the BroadView Agent running on a switch system. The Analytics application typically runs outside the switch system, in an x86 server and uses REST API exported by the BroadView Agent. 

BroadView Analytics provides the ability to visually manage and monitor various switches running BroadView Agent. Built on top of the BroadView Instrumentation Library, the BroadView Analytics application supports device management as well as managing individual BroadView features supported by the switch. The Analytics application gathers data from the BroadView Agent to enable several advanced use cases such as micro-burst detection, aggregation group optimization, packet path tracing, IPFIX based flow monitoring etc.

Built as a multi-window application, it allows simultaneous monitoring of various data that user is interested in, while providing visual indication of any critical events occurring at the devices. BroadView Analytics application persistently stores any important switch configuration and restores the previous configuration upon an application restart.  It also provides time-stamped logs to facilitate detailed analysis of raw data.

## Supported Features
- **Switch Registration** BroadView Analytics supports automatic registration and manual registration of BroadView enabled Switches. The registered Switches can be configured to monitor various supported instrumentation features.

- **Buffer Statistics Tracking (BST)** enables pro-active monitoring of buffer occupancies through "pushed" or "pulled" reports. It also supports threshold based congestion monitoring and micro-burst detection.

- **Congestion Drop Counters** allows to monitor for top ports suffering congestion or monitor the number of packets dropped due to congestion, on a per-port, per-queue-type (broadcast or multicast), or per-port-per-queue.

- **Packet Tracing & Injection (PTI)** enables user to inject debug packets and capture trace profile that provides visibility into how the packet was processed in the switch pipeline. Aggregation group optimization is one good use case for this feature.

- **Live Packet Tracing & Injection (Live-PTI)** allows user to configure the Switch for obtaining packet distribution across 'LAG' or 'ECMP', the user interface allows user to match incoming packets against a user-specified match criterion (5-Tuple). Packet path tracing, basic latency analysis and advanced troubleshooting are some use cases of this feature.

- **Flow Tracker (FT)** enables IPFIX based flow monitoring where packet flow statistics are gathered based on inspecting every packet (not sampled).

Documentation
=============

BroadView Analytics user guide can be found at [doc] (doc)

Legal
=====

Please see LEGAL_TERMS for the use of and access of the Broadcom-Switch Page

License
=======

Licenses for the software are available at the applicable level of the
software repository under the "LICENSE" file

