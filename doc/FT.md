Flow Tracker
=====================
The Flow Tracker feature provides deep visibility of IP flows passing through the Switch silicon. The feature allows user to configure 5-tuple for which the flows should be monitored. It is possible to use wildcards for some parameters of the 5-tuple. The feature also allows user to configure flows destined to pass through the specified egress ports. The BroadView Analytics application facilitates the configuration of the BroadView Agent to export IPFIX records (Flow-related metrics that are captured within the ASIC) to remote collector application at regular intervals.

`Note: To use complete functionality offered by Flow Tracker feature, IPFIX Collector is required to interpret the IPFIX records sent by the Switch.`

