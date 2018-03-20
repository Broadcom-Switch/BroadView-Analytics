Monitoring On-Chip Buffers
==========================
The BroadView Analytics application enables user to collect and analyze data from on-chip buffers. The ASIC has several features that allow a customer to monitor the internal details of chip buffers during runtime. The ASIC also provides the means to monitor buffer utilizations under a given traffic scenario. A collection of these buffer counts for the various buffers in the ASIC is called the buffer statistics tracking report. This report is sent by the BroadView agent to the BroadView Analytics application either on demand or periodically, based on user configuration. The feature to monitor on-chip buffers is enabled by default on the BroadView Analytics. When a switch is successfully registered (either manually or by using the auto-registration mechanism), the switch is checked periodically for reachability. In the BroadView Analytics application, the software also listens on a configured port (the default port is **9070**) for asynchronous notification messages like Buffer Statistics reports and auto-registration messages from the switches. The BroadView Analytics provides visibility to various reports to monitor and analyze. The reports include:

- Buffer Statistics Reports
- Threshold-Based Buffer Statistics Reports
- Congestion Drop Counters

