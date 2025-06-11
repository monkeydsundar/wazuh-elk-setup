# wazuh-elk-setup
Wazuh + Filebeat + Elasticsearch + Kibana setup guide for Cisco/Fortinet
# 🔍 Network Log Monitoring with Wazuh SIEM (Cisco & Fortinet)

A fully on-premises SIEM setup using **Wazuh**, **Filebeat**, **Elasticsearch OSS**, and **Kibana OSS**, built to collect and monitor real-time logs from Cisco Catalyst switches and FortiGate firewalls. This project demonstrates security engineering, syslog routing, and visualization expertise.

---

## 🎯 Use Case / Problem Statement

Organizations often lack centralized visibility into network device events like configuration changes, login attempts, and traffic anomalies. This project solves that gap by enabling real-time log collection, alerting, and analysis for key perimeter devices.

---

## 🧱 Architecture Overview

```
[ Cisco Catalyst 1000 ]     [ FortiGate 40F ]
          |                         |
          └──────┐      ┌──────────┘
                 ▼      ▼
              [ rsyslog (UDP 514) ]
                        |
                        ▼
                  [ Wazuh Manager ]
                        |
                        ▼
                   [ Filebeat OSS ]
                        |
                        ▼
               [ Elasticsearch OSS ]
                        |
                        ▼
                   [ Kibana OSS UI ]
```

---

## 🚀 Key Features

* ✅ Cisco switch syslog parsing
* ✅ FortiGate syslog integration
* ✅ Centralized logging with rsyslog
* ✅ Real-time alerts from Wazuh rules
* ✅ Log indexing and search via Elasticsearch
* ✅ Dashboards and filters in Kibana

---

## 📂 Project Files

| File Name                 | Purpose                              |
| ------------------------- | ------------------------------------ |
| `Wazuh(FB+ELSTK+KIB).pdf` | Full step-by-step installation guide |
| `README.md`               | Project portfolio summary            |

---

## 🛠️ Tools & Technologies

* **Wazuh** 4.7.3 – Threat detection and alert engine
* **Filebeat OSS** 7.10.2 – Log shipping
* **Elasticsearch OSS** 7.10.2 – Log indexing
* **Kibana OSS** 7.10.2 – Log visualization
* **rsyslog** – Syslog forwarder from network devices
* **Ubuntu Server** 22.04 – Base OS

---

## 🎓 Skills Demonstrated

* Network security log parsing
* Linux server administration
* rsyslog-based log routing
* SIEM alert rule creation
* Visualization building in Kibana
* Troubleshooting live syslog feeds

---

## ✅ Results

* Real-time alerts generated for:

  * Configuration changes
  * Login/logout attempts
  * Network anomalies
* Functional dashboards for:

  * Traffic trends
  * Firewall actions
  * Syslog severity over time

---

## 🧠 What I Learned

* The challenges of parsing different vendor log formats
* Using Filebeat to decouple data shipping from the analysis engine
* Fine-tuning Wazuh rules for actionable alerts
* Building visually clean and meaningful dashboards in Kibana

---

> 📌 This project demonstrates hands-on SIEM setup from scratch and is suitable for showcasing in a security engineer portfolio.

---


