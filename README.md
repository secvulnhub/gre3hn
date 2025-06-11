# 🛡️ gre3hn

<div align="center">

**Linux Anonymous Shield**  
*Multi-distro anonymization tool with Tor, I2P, MAC randomization*

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Linux](https://img.shields.io/badge/OS-Linux-green.svg)](https://www.linux.org/)
[![Bash](https://img.shields.io/badge/Shell-Bash-4EAA25.svg)](https://www.gnu.org/software/bash/)
[![Python](https://img.shields.io/badge/Python-3.6%2B-3776AB.svg)](https://www.python.org/)

*Protecting your digital footprint across all major Linux distributions*

![gre3hn Demo](https://via.placeholder.com/800x400/1a1a1a/00ff00?text=gre3hn+Anonymous+Shield)

</div>

---

## ✨ Features

<table>
<tr>
<td width="50%">

### 🔐 **Core Anonymization**
- **Tor Integration** - Optimized configuration with transparent proxy
- **I2P Support** - Additional anonymity layer for enhanced protection  
- **MAC Randomization** - Hardware fingerprint protection
- **Secure DNS** - Prevents DNS leaks with trusted resolvers
- **Firewall Kill Switch** - Blocks non-anonymous traffic automatically

</td>
<td width="50%">

### 🐧 **Universal Compatibility**
- **Arch Linux** (pacman)
- **Ubuntu/Debian** (apt)
- **RHEL/CentOS/Fedora** (yum/dnf)
- **openSUSE** (zypper)
- **Gentoo** (emerge)
- **Alpine Linux** (apk)

</td>
</tr>
</table>

### 🚀 **Advanced Features**
- Bridge support for censored networks
- Real-time status monitoring
- System performance optimizations
- Automatic restoration on exit
- Comprehensive logging and diagnostics

---

## 📋 Prerequisites

- Linux distribution (any supported distro)
- Root/sudo access
- Basic network connectivity
- Minimum 1GB RAM recommended

---

## 🔧 Installation

### Quick Setup

```bash
# Download and make executable
wget https://raw.githubusercontent.com/user/gre3hn/main/gre3hn
chmod +x gre3hn

# Install dependencies (auto-detects your distro)
sudo ./gre3hn install

# Apply system optimizations (optional but recommended)
sudo ./gre3hn optimize
```

### Manual Installation

```bash
# Clone the repository
git clone https://github.com/user/gre3hn.git
cd gre3hn

# Make executable
chmod +x gre3hn

# Install dependencies
sudo ./gre3hn install
```

---

## 🚀 Quick Start

### Basic Usage

```bash
# Start anonymous shield
sudo ./gre3hn start

# Check status
./gre3hn status

# Stop shield and restore settings
sudo ./gre3hn stop
```

### Advanced Usage

```bash
# Monitor in real-time
sudo ./gre3hn monitor

# Configure settings
./gre3hn config

# Setup bridges for censored networks
sudo ./gre3hn bridges

# Test anonymity
./gre3hn test
```

---

## ⚙️ Configuration

The configuration file is automatically created at `~/.anon_shield/config.conf`:

```ini
[general]
auto_start_tor=true
auto_start_i2p=false
randomize_mac=true
secure_dns=true
kill_switch=true
stealth_mode=false

[tor]
socks_port=9050
control_port=9051
dns_port=9053
trans_port=9040
use_bridges=false

[dns]
primary=1.1.1.1
secondary=8.8.8.8
fallback=9.9.9.9
```

### Editing Configuration

```bash
# Open configuration editor
./gre3hn config
```

---

## 📊 Status Monitoring

<details>
<summary><strong>View Sample Status Output</strong></summary>

```
    ╔══════════════════════════════════════════╗
    ║        Anonymous Network Shield          ║
    ║      Universal Linux Privacy Tool        ║
    ╚══════════════════════════════════════════╝

✓ Tor: Running on port 9050
✓ I2P: Running on port 4444
✓ MAC Addresses: Randomized
  eth0: 02:42:ac:11:00:02
  wlan0: 02:42:ac:11:00:03
✓ DNS: Secured
✓ Firewall: Active (Kill Switch Enabled)

ℹ Testing anonymity...
✓ Tor IP: 185.220.101.32
✓ Kill Switch: Working (direct connections blocked)
```

</details>

---

## 🌐 Network Configurations

### Standard Configuration
Perfect for general anonymity needs with Tor routing.

### Censorship Circumvention
Uses bridges to bypass network restrictions in countries with internet censorship.

```bash
# Setup bridges for censored networks
sudo ./gre3hn bridges
```

### High Security Mode
Enables stealth mode with additional security measures.

```ini
[general]
stealth_mode=true
kill_switch=true
```

---

## 🛠️ Commands Reference

| Command | Description | Requires Root |
|---------|-------------|---------------|
| `install` | Install dependencies for your distribution | ✅ |
| `start` | Activate anonymous shield | ✅ |
| `stop` | Deactivate shield and restore settings | ✅ |
| `restart` | Restart the shield | ✅ |
| `status` | Show current anonymization status | ❌ |
| `config` | Edit configuration file | ❌ |
| `optimize` | Apply system performance optimizations | ✅ |
| `cleanup` | Remove system optimizations | ✅ |
| `bridges` | Configure Tor bridges | ❌ |
| `monitor` | Real-time status monitoring | ❌ |
| `test` | Test anonymity and connectivity | ❌ |
| `help` | Show help information | ❌ |

---

## 🔒 Security Features

### MAC Address Randomization
Changes hardware identifiers to prevent device tracking across networks.

### DNS Security
- Prevents DNS leaks through secure resolvers
- Automatic backup and restoration
- Immutable configuration during active session

### Traffic Routing
- All HTTP/HTTPS traffic routed through Tor
- Transparent proxy configuration
- Kill switch prevents non-anonymous connections

### Firewall Protection
- Blocks direct internet connections when active
- Only allows traffic through anonymization networks
- Automatic rule cleanup on exit

---

## 🌍 Distribution Support

<details>
<summary><strong>Arch Linux</strong></summary>

```bash
# Packages installed via pacman
- tor
- i2pd
- python-psutil
- iptables
- iproute2
```

</details>

<details>
<summary><strong>Ubuntu/Debian</strong></summary>

```bash
# Packages installed via apt
- tor
- i2p
- python3-psutil
- iptables
- iproute2
- curl
```

</details>

<details>
<summary><strong>RHEL/CentOS/Fedora</strong></summary>

```bash
# Packages installed via dnf/yum
- tor
- python3-psutil
- iptables
- iproute
- curl
```

</details>

---

## 🧪 Testing Your Setup

### Verify Tor Connection
```bash
# Test Tor connectivity
curl --socks5 127.0.0.1:9050 https://check.torproject.org/api/ip
```

### Check for Leaks
```bash
# Run comprehensive anonymity test
./gre3hn test
```

### Monitor Real-time
```bash
# Continuous monitoring
sudo ./gre3hn monitor
```

---

## 📂 File Structure

```
~/.anon_shield/
├── config.conf          # Main configuration
├── shield.log           # Activity logs
├── torrc                # Tor configuration
├── tor_data/            # Tor data directory
├── original_macs.json   # MAC address backup
└── dns_backup           # DNS configuration backup
```

---

## 🚨 Important Security Notes

**⚠️ Root Access Required**  
This tool requires root privileges to modify network settings, MAC addresses, and firewall rules.

**🔄 Automatic Restoration**  
All changes are automatically reverted when stopping the shield, including:
- Original MAC addresses
- DNS configuration
- Firewall rules
- System optimizations

**🛡️ Kill Switch Protection**  
When active, the kill switch prevents any non-anonymous traffic, ensuring your real IP is never exposed.

**🌐 Bridge Networks**  
For users in censored networks, bridges provide alternative connection methods to the Tor network.

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit pull requests, report bugs, or suggest features.

### Development Setup
```bash
git clone https://github.com/0xb0rn3/gre3hn.git
cd gre3hn
chmod +x gre3hn
```

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## ⚠️ Disclaimer

This tool is for educational and privacy protection purposes. Users are responsible for complying with local laws and regulations. The developers are not responsible for any misuse of this software.

---

<div align="center">

**Made with ❤️ for the privacy community**

[Report Bug](https://github.com/user/gre3hn/issues) • [Request Feature](https://github.com/user/gre3hn/issues) • [Documentation](https://github.com/user/gre3hn/wiki)

</div>
