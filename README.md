# 🔓 HexAir
**Wireless Auditing & Security Testing Toolkit for Kali Linux**

HexAir is a powerful, menu-driven wireless assessment tool that automates monitor mode setup, network scanning, and provides a comprehensive suite of attacks including handshake capture, cracking, deauthentication, DoS/DDoS, Evil Twin, and brute-force password attacks.

---

## ✨ Features

- ✅ Automatic monitor mode detection & setup
- 📡 Scan & display all nearby Wi-Fi networks
- 🎯 Target selection from discovered networks
- 🔑 Capture WPA/WPA2 handshake
- 🔓 Crack captured handshake with dictionary/wordlist
- 💥 Deauthentication (Deauth) attack
- 🌊 DoS / DDoS attacks on target network
- 🧪 Evil Twin access point creation
- 🔢 Brute-force password attack
- 🎨 Interactive CLI with numbered options

---

## 📋 Prerequisites

- **Kali Linux** (recommended) or any Debian-based distro with wireless tools
- **External Wi-Fi adapter** that supports monitor mode and packet injection
- Root privileges

---

## 🚀 Installation

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


```bash
sudo apt update
sudo apt install aircrack-ng mdk4 hostapd dnsmasq wordlists -y
```

🛠 Usage

1. Run the tool as root:

sudo bash wifi_pentest.sh

1. The tool will:
   · Check for monitor mode capability and enable it automatically
   · Scan for available Wi-Fi networks and display them with numbers
   · Prompt you to select a target by number
2. After selecting a target, you'll see the main menu:

```
[1] Capture Handshake
[2] Crack Handshake (requires .cap file)
[3] Deauth Attack
[4] DoS Attack
[5] DDoS Attack
[6] Evil Twin
[7] Brute Force Password Attack
[8] Exit
```

📸 Example

```
$ sudo bash wifi_pentest.sh

[*] Checking wireless interfaces...
[+] Monitor mode enabled on wlan0mon.
[*] Scanning networks. Press Ctrl+C when done...

Available networks:
1) HomeWiFi - 2C:30:33:12:4A:B1 (CH 6)
2) NeighborNet - 6A:12:3F:22:BC:44 (CH 1)

Select target number: 1

Target: HomeWiFi [2C:30:33:12:4A:B1]

=== Main Menu ===
[1] Capture Handshake
[2] Crack Handshake
[3] Deauth Attack
[4] DoS Attack
[5] DDoS Attack
[6] Evil Twin
[7] Brute Force Password Attack
[8] Exit

Choice:
```

---

⚠️ Legal Disclaimer

HexAir is intended for educational purposes and authorized security testing only. Unauthorized use against networks you do not own or have explicit permission to test is illegal. The author assumes no liability for misuse or damage caused by this tool.

---

🤝 Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your improvements or new features.

---

📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

---

━━━━━━━━━━━━━━━━━━━━━━━━━━━━
🐣 Project by neel470
━━━━━━━━━━━━━━━━━━━━━━━━━━━━


