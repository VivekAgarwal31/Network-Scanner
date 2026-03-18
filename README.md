# 🛡️ Interactive Network Security Scanner

![MIT License](https://img.shields.io/badge/License-MIT-green.svg)

## 🚀 Overview

A robust, menu-driven terminal network scanner designed for system administrators, cybersecurity learners, and penetration testers. Features automatic local IP detection, threaded scanning, vulnerability insights, and a clean UI—all in an interactive Python package.  

**Author:** Vivek Agarwal

---

## 🎯 Features

- 🔍 **Quick Scan:** Fast port scan of common ports (1-1024)
- 🔎 **Full Scan:** Comprehensive scan of all ports (1-65535)
- ⚙️ **Custom Scan:** User-defined port ranges
- 📊 **Vulnerability Assessment:** Highlights risky/critical services based on port and protocol
- 🌐 **Network Info:** Local IP/interface and default gateway lookup
- 📋 **Multithreaded Engine:** 50-500 threads for fast, stable scanning
- 💾 **JSON Reports:** Automated exports of scan results and vulnerabilities
- ❗ **Built-in Help/Settings:** Easily accessible usage and configuration docs
- ✅ **Banner Grabbing & SSL Checks:** Extract HTTP/S, SMTP banners and test for SSL/TLS info on specific ports

---

## 🛠️ Installation

1. **Clone the Repository**

    ```
    git clone https://github.com/UJ2406/Network_Scanner.git
    cd Network_Scanner
    ```

2. **Python 3.6+ Required**  
    Recommended: Python 3.8 or higher

3. **Install Dependencies**  
    All dependencies are from the Python standard library (no pip needed!):
    - `socket`
    - `threading`
    - `json`
    - `ssl`
    - `datetime`
    - `subprocess`
    - `os`
    - `re`
    - `concurrent.futures`

    *No external modules required.*

4. **Run the Tool**

    ```
    python3 nsc.py
    ```

---

## 🖥️ Usage

- Launch script and use the interactive menu to:
    - Quick, full, or custom port scan a host/IP
    - Review open ports and matched vulnerabilities (auto-suggested by port)
    - Show network/interface details
    - Configure scanning options (thread count, port range)
    - Export scan results as a JSON report
- Full help and safety tips are built into the interface (`Help` menu).

---

## 📝 Example Menu 

```
╔══════════════════════════════════════════════════════════════╗
║ 🛡️ NETWORK SECURITY SCANNER 🛡️                              ║
║ Professional Security Assessment Tool                        ║
╚══════════════════════════════════════════════════════════════╝

🔍 Quick Scan (Ports 1-1024)​
🔎 Full Scan (Ports 1-65535)​
⚙️ Custom Scan (Choose Range)​
🌐 Scan Local Network​
📊 View Network Info​
⚙️ Settings​
📖 Help​
🚪 Exit
```


---

## 📦 Output

- **Live port scan summaries to terminal**
- **Vulnerability report** (auto-detected)
- **Optional JSON export:**  
  Contains open ports, service banners, SSL/TLS info, matched vulnerability details, and summary breakdown.

---

## 🔒 Security Concepts Learned

- **Port scanning**: Identifying service exposure and initial attack surface
- **Vulnerability mapping**: Matching open ports to known high-risk services
- **Banner grabbing**: Collecting version information—vital for exploit research
- **SSL/TLS check**: Surface level certificate/cipher info for common secure protocols
- **Multithreading**: Efficient parallel scanning to minimize total scan time
- **Network hygiene**: Seeing real security posture, not just theoretical exposure

---

## 🧩 Good to Know / Best Practices

- Run with permission only—**unauthorized scanning is illegal!**
- For best results, scan a target on the same network or properly configured external host ("scanme.nmap.org" is safe for testing).
- Increase thread count for speed, but be mindful of DoS/false positives.
- Full range scans (1-65535) may take longer—limit range for targeted/efficient checks.
- For deep vulnerability scanning, follow up with specialized tools (e.g., Nessus, OpenVAS).

---


## ❗ Legal/Ethical Notice

- **Only scan assets/networks you own or have written permission to assess.**
- Misuse is illegal and against community guidelines.

---

## 👤 Author

- **Vivek Agarwal**
- email - vivekagrawal6336@gmail.com
- Cybersecurity student  
- https://tryhackme.com/p/LuciferVivek31

---

## 📂 Repository Structure

```
network-scanner/
├── nsc.py                       # Main Scanner Script
├── demo_scan_report.json        # Scan report of hackthesite
├── README.md                    # This file
└── Screenshots                  # Demo images
└── LICENSE                      # MIT License
```

## 📜 License

This project is licensed under the [MIT License](LICENSE).  
You are free to use, modify, and distribute this software with proper attribution.
