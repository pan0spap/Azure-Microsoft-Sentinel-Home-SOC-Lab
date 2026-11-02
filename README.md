# Azure-Microsoft-Sentinel-Home-SOC-Lab

## Project Overview

In this project, I built a Home SOC Lab using Microsoft Azure and Microsoft Sentinel to monitor and investigate suspicious login activity.

I deployed a Windows Virtual Machine as a honeypot, collected security logs, and analyzed failed login attempts to identify potential malicious activity.

I also added a geographical attack map and MITRE ATT&CK mapping based on failed login events.


## Tools & Technologies

- Microsoft Azure
- Windows Virtual Machine
- Azure Monitor Agent (AMA)
- Log Analytics Workspace
- Microsoft Sentinel
- Kusto Query Language (KQL)
- MITRE ATT&CK Framework

## Project Architecture

1. **Deploy a Windows VM** in Microsoft Azure.
2. **Collect Windows Security Events** from the virtual machine.
3. **Forward logs** to Log Analytics Workspace.
4. **Analyze failed login attempts** using Microsoft Sentinel and Kusto Query Language (KQL).
5. **Visualize attacker IP geolocations** using an attack map.
6. **Map relevant security activity** to the MITRE ATT&CK Framework.


```mermaid
flowchart TD
    A["Internet"] --> B["Azure"]
    B --> C["Windows VM (Honeypot)"]
    C --> D["Windows Security Logs"]
    D --> E["Azure Monitor Agent"]
    E --> F["Log Analytics Workspace"]
    F --> G["Microsoft Sentinel"]
    G --> H["KQL Queries"]
    H --> I["Failed Login Analysis"]
    I --> J["Attack Map"]
    I --> K["MITRE ATT&CK Mapping"]
