# Network-Based Intrusion Detection System Using Snort

**Author:** [Your Name]  
**Environment:** Kali Linux (Oracle VirtualBox)  
**Tool Used:** Snort (Open-Source NIDS)  
**Classification:** Educational / Portfolio Project

---

## 1. Introduction

With the growing complexity and volume of cyber threats, ensuring the security of computer networks has become a significant concern. One essential defense mechanism in modern network security is the Intrusion Detection System (IDS), which helps identify unauthorized access and malicious activities within a network environment.

This project focuses on a Network-Based Intrusion Detection System (NIDS), designed to monitor traffic across a network in real time. Unlike host-based systems, NIDS analyze data packets as they move through the network infrastructure, making them effective in detecting threats such as scanning, spoofing, and exploitation attempts.

**Snort**, a popular open-source NIDS developed and maintained by Cisco, was used for this project. Snort captures network traffic and compares it against a set of predefined rules to detect abnormal or harmful behavior, functioning as a packet sniffer, logger, and real-time intrusion detector.

---

## 2. Motivation

- **Evolving Threats** — conventional security measures are increasingly inadequate against sophisticated attacks.
- **Cost-Effectiveness** — Snort is a free, open-source solution.
- **Customization** — rule-based detection can be tailored to specific network environments and threat types.

---

## 3. Scope

The scope of this project includes:

- Deployment of Snort in a test network environment for real-time traffic analysis.
- Configuration and customization of Snort rules to detect specific types of network-based intrusions.
- Monitoring and logging of network traffic, with alerts generated upon detection of anomalies or malicious behavior.
- Analysis of detected threats to understand attack patterns and improve network defenses.

---

## 4. Lab Setup

### 4.1 Installing Kali Linux on Oracle VirtualBox

**Prerequisites:**
- Oracle VirtualBox installed ([virtualbox.org](https://www.virtualbox.org))
- Kali Linux ISO ([kali.org](https://www.kali.org))

**Steps:**
1. Download the Kali Linux ISO (64-bit recommended) from the official site.
2. Open VirtualBox → click **New**.
3. Configure VM settings:
   - Name: `Kali Linux`
   - Type: `Linux`
   - Version: `Debian (64-bit)`
4. Complete VM configuration and boot into Kali.
5. Login with default credentials: `kali / kali`

| Step | Screenshot |
|---|---|
| Kali download page | ![Kali Webpage](./screenshots/fig1-kali-webpage.jpg) |
| Pre-built VM options | ![Pre-built VMs](./screenshots/fig2-prebuilt-vms.jpg) |
| VirtualBox Manager | ![VirtualBox Manager](./screenshots/fig3-virtualbox-manager.jpg) |
| Kali login screen | ![Kali Login](./screenshots/fig4-kali-login.jpg) |
| Kali desktop | ![Kali Desktop](./screenshots/fig5-kali-desktop.jpg) |

---

### 4.2 Installing Snort on Kali Linux

**Step 1 — Install Snort:**
```bash
sudo apt install snort
