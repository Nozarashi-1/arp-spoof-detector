# ARP Spoof Detector 

This Python tool detects **ARP spoofing / ARP poisoning** attacks in real time.  
It works by sniffing ARP packets on the network and comparing the actual MAC address of a host with the one announced in ARP replies. If they do not match, it warns you that you may be under attack.

---

## ⚠ Disclaimer
    This tool is intended for **authorized network monitoring and educational purposes only.  
    Do NOT use it for malicious activities. Unauthorized use is illegal.

---

## 📌 Features
- Detects ARP spoofing attempts in real time
- Compares claimed MAC address with the actual MAC address
- Works in **Python 2**
- Lightweight — runs continuously with minimal system load

---

## 🛠 Installation

**1. Clone the repository:**
```bash
git clone https://github.com/yourusername/arp-spoof-detector.git
cd arp-spoof-detector
```

## 🚀 Usage
Run the script with root privileges:
```bash
sudo python arp_spoof_detector.py
```
By default, the interface is hardcoded to:
``` bash
sniff("eth0")
