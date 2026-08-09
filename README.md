# Cisco NetFlow Traffic Analysis & Network Security Monitoring

A Cisco Packet Tracer implementation demonstrating network flow monitoring, traffic baselining, and anomaly detection using the Cisco NetFlow protocol.

## Overview
NetFlow provides granular visibility into IP network traffic flows as they traverse core interfaces. This lab demonstrates real-time telemetry exporting from an edge router to a dedicated monitoring collector.

## Topology & Components
- **Edge Router (NetFlow Exporter):** Tracks flow records across internal (`GigabitEthernet0/0`) and WAN interfaces (`Serial0/0/1`).
- **Internal Network (`10.0.0.0/24`):** Client endpoints generating HTTP traffic across the edge perimeter.
- **External Web Server (`192.0.2.100`):** Target destination simulating internet-bound traffic flows.

## Cisco IOS CLI Verification
```text
Edge# show ip cache flow
