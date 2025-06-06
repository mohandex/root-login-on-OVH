# Root Login on OVH – SSH Configuration Script

A Bash script to configure SSH access on Linux servers hosted on OVH, allowing root login with password authentication and disabling public key authentication.

> Author: [@mohandex](https://github.com/mohandex)

## 🔧 What This Script Does

- Verifies if the script is being run as root
- Prompts the user to set a new root password
- Replaces the content of `/etc/ssh/sshd_config` with custom secure settings
- Removes all files from `/etc/ssh/sshd_config.d/`
- Reloads the SSH service to apply the changes

## ⚠️ Warning

⚠️ **Important**: This script completely overwrites your existing SSH config and deletes all files in `/etc/ssh/sshd_config.d/`.  
Make sure to **back up your current SSH configuration** before running it.

---

## 🚀 Quick Install (One-liner)

> ⚠️ Use this method **only if you trust the contents of the script**  

🛠 Manual Installation
```bash
git clone https://github.com/mohandex/root-login-on-OVH.git
cd root-login-on-OVH
chmod +x script
sudo ./script
```

✅ Compatibility
Tested on:

Ubuntu 20.04 / 22.04

Debian 10 / 11

CentOS 7 / 8

📃 License
MIT License – you are free to use, modify, and distribute this script.

