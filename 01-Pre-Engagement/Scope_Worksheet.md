# Scope Definition Worksheet

> This document defines the technical boundaries of the engagement. Please list all assets to be tested.

## 1. Target Information

### A. Web Applications / URLs
| Application Name | URL | Environment (Prod/Staging) | Role needed? (Admin/User) |
| :--- | :--- | :--- | :--- |
| e.g., Main Portal | https://portal.company.com | Staging | Yes, 2 roles |
| | | | |

### B. IP Ranges / Network
| Description | IP Address / CIDR | Hosting Provider (AWS/Azure/On-prem) |
| :--- | :--- | :--- |
| e.g., VPN Gateway | 192.168.1.1 | On-premise |
| | | |

## 2. Exclusions (Do Not Attack)
*List any IP or specific subdomain that strictly CANNOT be tested.*
1. __________________________
2. __________________________

## 3. Technical Constraints
* **WAF/IPS:** Is there an active firewall? (Yes/No)
    * *If Yes, should we whitelist the Pentester's IP?* (Yes/No)
* **Cloud:** Do we need to notify the Cloud Provider? (Yes/No)

## 4. Objectives (Flags)
What is the main goal?
- [ ] Find as many vulnerabilities as possible.
- [ ] Prove access to a specific database (PII).
- [ ] Test the Blue Team's detection capabilities.
