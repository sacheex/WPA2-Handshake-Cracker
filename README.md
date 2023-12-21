# WPA2-Password-Cracker


This repository contains a Bash script for catching WPA2 4-way handshake using Aircrack-ng tools. The script automates the process of capturing BSSID and Handshake for a specified Wi-Fi network.


# Disclaimer

This project is a demonstration and educational tool developed for learning and research purposes only. The primary goal is to provide insights into network security and cryptography by showcasing the vulnerabilities associated with weak handshake protocols.


**Note: Unauthorized access to computer systems and networks is illegal and unethical. This project should only be used in environments where you have explicit permission to test and assess security.**


## Installation

#### Make sure you have Aircrack-ng and gnome-terminal installed. You can install them on Debian-based systems using:

```bash
sudo apt update
sudo apt install aircrack-ng
sudo apt install gnome-terminal
```
#### Clone the repo and navigate to the directory
```bash
git clone https://github.com/your-username/wifi-hacking-script.git
cd WPA2-Password-Cracker
```
#### Make the script executable
```bash
chmod +x wifi-hack.sh
```

#### Run the script
```bash
./handshakeCatcher.sh
```

## Crack the password

Use Wireshark to open the captured file. Make sure you capture the 4-way handshake.

```bash
wireshark <filename>.cap
```
Filter wireshark messages for eapol

#### Use Aircrack-ng to crack the password. Provide a password list, such as rockyou.txt, for brute force.

```bash
aircrack-ng <filename>.cap -w <path to password list>
```

Feel free to customize the content further based on your preferences or additional information you want to include in the README.
