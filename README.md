# Kali-Pentbox-Honeypot-Lab
A local attack and defense simulation using a Pentbox honeypot on port 23 (Telnet) and Kali Linux.
# Local Attack & Defense Lab: Pentbox Honeypot Deployment

## Project Overview
This project demonstrates the deployment of a local network honeypot to detect, log, and analyze adversarial reconnaissance and unauthorized access attempts. Operating entirely within an isolated virtual environment, I simulated a malicious actor probing a target network via Telnet, allowing me to evaluate the effectiveness of deception-based defense mechanisms.

---

## 🛠️ Skills & Technologies Demonstrated
* **Deception Technology:** Deploying and configuring a network honeypot listener using Pentbox.
* **Network Exploitation & Interaction:** Simulating an active connection attempt on unencrypted legacy protocols (Telnet).
* **Incident Logging & Analysis:** Analyzing real-time intrusion alerts to extract attacker signatures (Source IP and Port).
* **Virtual Network Isolation:** Using a secure virtual network environment to safely capture and analyze malicious traffic.

---

## 🔍 The Simulation: Step-by-Step

### 1. Attacker Connection Attempt
From the Kali Linux attacker machine, I simulated a reconnaissance and access attempt by targeting the commonly exploited Telnet service on Port 23.
```bash
telnet <Honeypot_IP>
```
### 2. Honeypot Activation & Intrusion Logging
The moment the connection request hit the target machine, the Pentbox honeypot successfully tripped, dropped the connection/spoofed a response, and logged the signature.

## 📊 Caught in the Act: Honeypot Alerts
Extracted Attacker Data:

Attacker IP: 10.0.2.15 (Kali Linux VM)

Targeted Port: Port 23 (Telnet)

Alert Status: HONEYPOT ACTIVATED
---

## 🏁 Conclusion
By configuring a local honeypot on Port 23, I successfully demonstrated how security teams can use active deception to catch malicious network behavior early in the cyber kill chain. This project highlights the core fundamentals of network monitoring, alert analysis, and defensive architecture.
