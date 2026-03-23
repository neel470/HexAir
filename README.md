# HexAir - Advanced WiFi Pentesting Framework

[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Kali Linux](https://img.shields.io/badge/platform-Kali%20Linux-black.svg)](https://www.kali.org/)
[![Aircrack-ng](https://img.shields.io/badge/tools-aircrack--ng-orange.svg)](https://www.aircrack-ng.org/)

**HexAir** is a production-ready WiFi penetration testing framework for Kali Linux. Automatically detects monitor-capable interfaces, scans networks, and provides complete attack suite: handshake capture/cracking, deauth/DoS/DDoS, WPS Pixie Dust, Evil Twin.

## ✨ Features

- ✅ Auto Interface Detection (monitor mode)
- 🔍 Real-time Network Scanning (BSSID/Channel/ESSID)
- 🤝 WPA2 Handshake Capture + Cracking
- ⚡ WPS Pixie Dust (CVE-2011-1547)
- 💥 Deauth/DoS/DDoS Attacks
- 👥 Evil Twin Rogue AP
- 🧹 Auto Cleanup

## 📦 Installation

```bash
# 1. Clone repository
git clone https://github.com/neel470/HexAir.git
cd HexAir

# 2. Make executable
chmod +x wifi_pentest.sh

# 3. Install dependencies (Kali default)
sudo apt update && sudo apt install -y aircrack-ng hashcat hcxtools

# 4. Run as root
sudo ./wifi_pentest.sh

🚀 Quick Start



[+] wlan0 supports monitor mode
[+] Scanning networks...
0: MyWiFi | AA:BB:CC:DD:EE:FF | 36 | -45dBm

1. Capture Handshake    4. Deauth Attack
2. Crack Handshake      5. DoS (ARP Replay)
3. Brute Force WPS      6. DDoS Multi-channel
7. Evil Twin AP         0. Exit

🛠️ Attack Modules


Module	Technique	Output Files
Handshake	Deauth + Capture	handshake-01.cap
Crack	Dictionary (rockyou.txt)	Cracked password
WPS Pixie Dust	Offline PIN	WPA key
Deauth	Frame Injection	Client disconnect
DoS	ARP Replay	Network flood
DDoS	Multi-channel	AP disruption
Evil Twin	Rogue AP	Client creds

📁 Structure



HexAir/
├── wifi_pentest.sh     # Main framework
├── README.md          # This file
└── LICENSE            # MIT License

⚠️ Legal Notice
Authorized pentesting only. For security assessments, red teaming, and owned networks.

📄 License
MIT License - see LICENSE [blocked] file


