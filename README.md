# Root Login on OVH – SSH Configuration Script

A Bash script to configure SSH access on Linux servers hosted on OVH, allowing root login with password authentication and disabling public key authentication.

> Author: [@mohandex](https://github.com/mohandex)

## 🔧 What This Script Does

- Verifies if the script is being run as root
- Prompts the user to set a new root password
- Replaces the content of `/etc/ssh/sshd_config` with custom secure settings
- Removes all files from `/etc/ssh/sshd_config.d/`
- Reloads the SSH service to apply the changes

## 📂 Files

- `my_script.sh`: The main Bash script

## ⚠️ Warning

⚠️ **Important**: This script completely overwrites your existing SSH config and deletes all files in `/etc/ssh/sshd_config.d/`.  
Make sure to **back up your current SSH configuration** before running it.

## 🚀 How to Use

1. **Clone the repository:**

   ```bash
   git clone https://github.com/mohandex/root-login-on-OVH.git
   cd root-login-on-OVH
   chmod +x script.sh
   sudo ./script.sh

You will be prompted to enter a new root password. After that, the script updates your SSH settings and reloads the SSH service.

✅ Compatibility
Tested on:

Ubuntu 20.04 / 22.04

Debian 10 / 11

CentOS 7 / 8



