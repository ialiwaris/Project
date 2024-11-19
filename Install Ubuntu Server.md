##  Installing-a-Ubuntu-Server
Step-by-step guide to install and configure a basic Ubuntu Server for beginners. This repository covers everything from downloading the ISO to setting up SSH, firewall, and essential tools for server management.
# Let's Install...
## ISO File: 
- [Download Ubuntu Server ISO](https://ubuntu.com/download/server)
## Bootable USB: A USB drive (minimum 4GB) and a tool like:
- [Rufus](https://rufus.ie/)
- [Balena Etcher](https://www.balena.io/etcher/)
## Hardware: Minimum 2GB RAM and 20GB of storage required...
# Install Ubuntu Server  
## 2. Creating a Bootable USB  
1. Download and install one of the following tools:  
   - [Rufus](https://rufus.ie/)  
   - [Balena Etcher](https://www.balena.io/etcher/)  
2. Connect your USB drive to your computer.  
3. Open the tool and:  
   - Select the downloaded [Ubuntu Server ISO](https://ubuntu.com/download/server).  
   - Format the USB and make it bootable.  
4. Once the process is complete, your USB is ready.  
---
## 3. Installing the Server  
### Boot into USB  
1. Restart your system and press `F2`, `F12`, `DEL`, or `ESC` to enter the BIOS/UEFI settings.  
2. Set the USB drive as the first boot priority.  
3. Save changes and reboot. The Ubuntu Installer will load.  
### Install Ubuntu Server  
1. Select your preferred language.  
2. Click **"Install Ubuntu Server"** to start the installation process.  
---
## 4. Installation Steps  
### Network Configuration  
- Select **DHCP** for automatic IP assignment or configure a static IP manually.  
### Storage Configuration  
- For disk partitioning, choose the default option: **Use entire disk**.  
### User Setup  
- Create an admin user by entering a username and password.  
- Specify the server's hostname (e.g., `myserver`).  
### SSH Setup  
- If you want remote access, install the SSH server during the setup process.  
### Installing Packages  
- Proceed with the default settings. You can install additional packages later as needed.  
---
## 5. Completing the Installation  
1. Restart the system after the installation is complete.  
2. Remove the USB drive.  
3. Your Linux server is now ready to use! 🎉  
# THANK YOU...
