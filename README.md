# 🛡️ Active Directory Security Lab

A hands-on lab setup to simulate real-world enterprise networks, built for learning **Active Directory**, **Windows Security**, **Attack Simulation**, and **SIEM Integration**.

---

## 🏗️ Lab Architecture

| Component         | Description                         | IP Address       |
|-------------------|-------------------------------------|------------------|
| Domain Controller | Windows Server 2022 (adlab.local)    | 192.168.10.7     |
| Client Machine    | Windows 10                          | 192.168.10.100   |
| Kali Linux Attacker | Kali Linux (Offensive tools)       | 192.168.10.250   |
| Splunk Server     | Splunk for log collection & analysis | 192.168.10.10    |

---

## 🔧 Configuration Overview

- **Domain Controller**: DNS, ADDS, Group Policy
- **Splunk Setup**: Universal Forwarder + Sysmon integration
- **Kali Linux**: Hydra, Nmap, BloodHound, Mimikatz for attacks
- **Static IPs** set on all machines for network stability
- **Bridged Network Mode** in VirtualBox

---

## 🧪 Attack & Defense Scenarios

| Attack Simulation      | Detection & Response           |
|-----------------------|--------------------------------|
| RDP Brute Force (Hydra) | Sysmon + Splunk alerts (T1110) |
| Credential Dumping (Mimikatz) | Sysmon Event ID 10 detection |
| PowerShell Execution (Atomic Red Team) | Splunk detection rules for T1059 |
| AD Enumeration (BloodHound) | Anomaly detection in logs |

---

##  Network Topology

![Image](https://github.com/user-attachments/assets/10ec854a-c028-4cac-8d00-8cff7149749b)

---

## 📊 Splunk Dashboards

📸 *Add screenshots of Splunk dashboards here!*  
_Example: RDP brute-force detection, PowerShell script monitoring, login anomalies._

---

## 📂 Files in This Repo

| File/Folder            | Purpose                                     |
|------------------------|---------------------------------------------|
| `/Screenshots`         | Lab setup, Splunk dashboards, attack demos   |
| `/Configurations`      | Sysmon config, Splunk inputs, GPO settings   |
| `/Notes`               | Lab notes, attack steps, detection findings  |
| `README.md`            | Project documentation                        |

---

## 📚 Learning Outcomes

✅ Configuring a **Domain Controller** from scratch  
✅ Setting up a **blue team lab** with Splunk & Sysmon  
✅ Executing **red team attack simulations**  
✅ Writing basic **detection rules** in Splunk  
✅ Understanding **networking in a virtual lab**

---

## 🚀 How to Reproduce This Lab

1️⃣ Install VirtualBox / VMware  
2️⃣ Create VMs (Windows Server, Windows 10, Kali)  
3️⃣ Configure static IPs, DNS, and AD  
4️⃣ Install Splunk and Sysmon  
5️⃣ Run Atomic Red Team tests and monitor in Splunk  
6️⃣ Simulate attacks with Hydra, BloodHound, Mimikatz  

---

## 🎓 Future Improvements

- Add Elastic Stack SIEM setup  
- Automate lab provisioning with scripts  
- Include cloud-based attack simulations  
- Integrate with Wazuh or other open-source tools

---

## 📬 Contact

🔗 [linkedin.com/in/gowri-shankar-ganesan-497944188](https://www.linkedin.com/in/gowri-shankar-ganesan-497944188)
✉️ gowrishankarganesan2513@gmail.com

---

