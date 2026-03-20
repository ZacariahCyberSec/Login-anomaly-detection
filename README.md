# 🔐 Login Anomaly Detection & Brute Force Analysis Lab

## 📌 Project Overview
This project simulates a Security Operations Center (SOC) scenario where suspicious login behavior is detected through log analysis using Python.

The goal is to identify:
- Unusual login times (late-night activity)
- Potential brute force attacks based on repeated failed login attempts

---

## 🛠️ Tools & Technologies
- Kali Linux
- Python 3
- VirtualBox
- Linux Authentication Logs (`auth.log`)

---

## 🔍 Scenario
A simulated SSH attack was performed, generating multiple failed login attempts from a single IP address.

The log data was analyzed to detect:
- Login attempts during unusual hours (00:00 – 05:00)
- Multiple failed login attempts from the same IP

---

## ⚙️ Detection Logic
The Python script performs:

- Reads and parses `auth.log`
- Extracts timestamps and IP addresses
- Identifies late-night login attempts
- Counts failed login attempts per IP
- Flags suspicious behavior

---

## 🚨 Detection Output
Example alerts generated:

[WARNING] Unusual login time detected from 192.168.1.50  
[ALERT] Possible brute force from 192.168.1.50 - 4 failed attempts  

---

## 📁 Project Structure
- anomaly_detector.py → Detection script  
- auth.log → Sample log data  
- screenshots/ → Execution and code proof  

---

## 🎯 Skills Demonstrated
- Log analysis & parsing  
- Threat detection (brute force & anomalies)  
- Python scripting for security automation  
- SOC investigation workflow simulation  

---

## 💡 Key Takeaways
- Identifying suspicious login patterns  
- Detecting anomalies in authentication logs  
- Building practical SOC-level detection scripts  

---

## 🚀 Future Improvements
- Detect new/unseen IP addresses  
- Add automated alert notifications (email)  
- Integrate with SIEM tools  

---

## 👨‍💻 Author
Tinashe Zacariah Nyandoro  
Aspiring SOC Analyst | Cybersecurity Enthusiast
