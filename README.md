# Firewall-Gui
# 🔥 Firewall Configuration on Windows and Linux (UFW)

🖼️ Screenshots (Placeholders)
 Screenshot of Windows Inbound Rule (Block Port 23)
![Image](https://github.com/user-attachments/assets/f3706ff9-992f-4db4-bd1e-c968e618585b)

## 🎯 Objective
To configure and test basic firewall rules to allow or block traffic on specific ports using:
Windows Defender Firewall
UFW (Uncomplicated Firewall) on Linux

## ✅ Outcome
Successfully blocked and tested traffic on Telnet port (23)
Allowed SSH traffic (port 22)
Validated and reverted changes
Understood how firewalls manage network traffic filtering

## ⚙️ Key Concepts
Firewall: Software that filters incoming and outgoing traffic based on rules
Ports: Logical endpoints for communication (e.g., 22 for SSH, 23 for Telnet)
UFW: Simple interface for managing iptables on Linux
Inbound/Outbound Rules: Define which traffic is allowed or blocked

## 🛠️ Steps Performed
### 🔹 Windows
1. Opened Windows Defender Firewall with Advanced Security
2. Created a new Inbound Rule to block port 23
3. Verified using telnet localhost 23
4. Deleted the rule

### 🔹 Linux (UFW)
1. sudo ufw enable                  # Enable firewall
2. sudo ufw deny 23                 # Block Telnet
3. telnet localhost 23              # Test blocked port
4. sudo ufw allow 22                # Allow SSH
5. sudo ufw delete deny 23          # Remove block rule

💬 Interview Questions 
1. What is a firewall?
2. Why block Telnet (Port 23)?
3. What is UFW?
4. How can you verify if a port is blocked?
5. What is ICMP and why block it?
6. What is SYN flood and firewall defense?
7. What is SPI?
