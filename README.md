# Active Directory

# 🛡️ Mini Cybersecurity Lab

This is a **mini cybersecurity lab**, a playground 🎢 for testing attacks and seeing how well they can be detected.

---

## 🔧 The Setup
This network, running under the **AJSOC** domain, has a few key components:

![Screenshot 2025-02-16 183128](https://github.com/user-attachments/assets/beb5f4fb-750d-415d-83e4-3e8a8f36c71f)
***Ref 1: Network Diagram***


1. **📊 Splunk Server (192.168.10.10)** – The security HQ 🏢. It collects logs from other machines, helping spot anything suspicious happening on the network.
2. **🖥️ Active Directory (192.168.10.7)** – The brain of the network 🧠, managing users and permissions. It also has Sysmon 🔍, a tool that tracks system activity and sends that information to Splunk.
3. **💻 Windows 10 Machine (IP: DHCP)** – A regular workstation, but with some extra tools:
   - 🔍 Sysmon (for logging system activity)
   - 📡 Splunk Universal Forwarder (sends logs to Splunk)
   - 💥 Atomic Red Team (used for simulating cyber attacks to test defenses)
4. **👨‍💻 Kali Linux (192.168.10.250)** – The hacker machine 🕵️‍♂️. This is the attacker in the setup, used to launch attacks and test security measures.
5. **🌐 The Network (Router & Switch)** – These connect everything together and allow traffic to flow between devices, just like in a real company network.

---

## ⚡ What This Lab Can Be Used For
- 🎭 **Simulating Cyber Attacks**: Using **Kali Linux** or **Atomic Red Team** to attempt hacking into the network.
- 🚨 **Detecting Threats**: Checking if **Splunk** catches the suspicious activity in the logs.
- 🔧 **Improving Security**: Adjusting settings, adding defenses, or fine-tuning detection rules based on findings.
- 🕵️‍♂️ **Threat Hunting**: Searching for indicators of compromise (IoCs) within collected logs.
- 🔑 **Privilege Escalation & Lateral Movement**: Testing how an attacker might move through the network and what security measures can detect or prevent it.

---

## 🛠️ Tools Used
- **Splunk** – Log collection and analysis
- **Sysmon** – Windows system monitoring
- **Kali Linux** – Penetration testing and ethical hacking
- **Atomic Red Team** – Adversary simulation
- **Active Directory** – User and access management
- **Splunk Universal Forwarder** – Sending logs from endpoints to Splunk

---

## 🛡️ Attack Scenarios
This lab can be used to simulate and detect different types of attacks, including:

- 🏴‍☠️ **Brute Force Attacks**: Attempting to crack passwords on Active Directory accounts.
- 🔗 **Phishing & Social Engineering**: Simulating credential harvesting techniques.
- 📡 **Lateral Movement**: Testing how an attacker can move from one machine to another.
- 🚀 **Privilege Escalation**: Identifying vulnerabilities that could allow an attacker to gain admin access.
- 🦠 **Malware Execution**: Running controlled malware samples to analyze detection capabilities.
- 🕵️ **Persistence Techniques**: Understanding how attackers maintain access to compromised machines.

---

## 🎓 Skills Learned
- **Threat Hunting**: Identifying and analyzing suspicious activity in logs.
- **Penetration Testing**: Using ethical hacking tools to simulate real-world attacks.
- **Incident Detection & Response**: Monitoring and responding to security events.
- **Log Analysis**: Understanding system and network logs for security insights.
- **Security Hardening**: Strengthening defenses against cyber threats.
- **SIEM (Security Information and Event Management) Operations**: Using Splunk to detect, investigate, and respond to threats.
- **Windows Security Monitoring**: Leveraging Sysmon for in-depth visibility into system events.
- **Network Traffic Analysis**: Capturing and analyzing network activity to detect potential intrusions.
- **Red vs. Blue Teaming**: Gaining experience from both an attacker's and defender's perspective.

---

This setup works like a **security camera system 🎥** for a house, but instead of burglars, it's designed to catch **hackers 🦹‍♂️**. Here, you can play both the **attacker and defender** to strengthen your cybersecurity skills!
