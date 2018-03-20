Tracing Packets across a LAG or ECMP Group
=====================
The packet trace feature provides a device-internal packet tracing mechanism. The feature allows to inject a packet into the ingress packet processing pipeline. The packet is then processed as if it was received on one of the front panel ports. During the trace, the feature logs information about egress hashing and traffic forwarding decisions. Upon completion, the packet trace feature provides information about how the packets were distributed across the ports that are members of the LAG or ECMP group.

BroadView Analytics packet trace feature to see how effectively the LAG or ECMP hashing algorithm is functioning for a particular traffic pattern. Using the BroadView Analytics, user can inject traffic into the ingress pipeline, and collect packet processing information.
The packet trace feature includes two options to get LAG/ECMP resolution:

- Inject a packet or packets in PCAP format to get the LAG/ECMP resolution.
- Create a live traffic triggered PTI profile and specify a 5-tuple (the match criteria). Then, initiate a request to the BroadView agent to get LAG/ECMP resolution for the packets matching the criteria. When a packet in the live traffic matches the specified criteria, the agent captures the LAG/ECMP resolution and sends the report to the BroadView Analytics application.

`Note: PCAP files with libpcap file format version 2.4 are supported`

