# Fedora 43 Installation Guide  

## 1 Overview  
This document explains steps involved in the installation of Fedora 43 on a UEFI-based x86_64 system
(typical PC/laptop). It involves a fresh installation (no upgrade) and includes steps of boot media
creation and installation.

## 2 Audience & Scope  
### 2.1 Who this is for  
This guide is intended for system administrators or users familiar with basic system hardware
BIOS/UEFI setup, who wish to install Fedora 43 as a workstation OS.  

### 2.2 What this covers  
* Downloading and verifying Fedora 43 installation media  
* Creating a bootable USB installation drive  
* Booting the installer  
* Basic installation: partitioning, user setup, software selection  
* First‑boot and initial configuration  
* Post‑installation tasks (updates, drivers, extras)  

### 2.3 What this does *not* cover  
* Complex storage setups (e.g., software RAID, network boot)  
* Server‑specific installations or custom Kickstart automation  
* Legacy BIOS-only systems  
* Spins or flavors of Fedora other than the default Workstation.

## 3 Prerequisites  
### 3.1 Hardware requirements (bare minimum) 
* Minimum 4 GB RAM (more is strongly recommended)  
* At least 20 GB of free disk space  
* UEFI firmware recommended; Secure Boot optional  

### 3.2 Download media  
* Visit the [Fedora download page](https://fedoraproject.org/workstation/download)  
* [Verify](https://jharaunak.medium.com/integrity-verification-1da85bb46457) the ISO checksum and GPG signature  

### 3.3 Bootable USB drive  
* Prepare a USB disk (8GB or higher) to serve as installation media.  
* On Windows/Mac/Linux, Rufus/Fedora Media Writer may be used.  

### 3.4 Firmware/BIOS settings  
* If installing alongside another OS, ensure you know the firmware boot mode (UEFI vs
BIOS) and whether the OS uses Secure Boot.  
* Optional: Disable Secure Boot or enroll keys if required for proprietary drivers.

## 4 Creating Installation Media  
### 4.1 Downloading the ISO  
* On the Fedora website, choose the “Workstation” edition for x86_64 architecture.  
* Save the ISO to the computer.  
* (Optional) Using the sha256sum or equivalent, compute the checksum and compare it with the
published one.  

### 4.2 Writing the ISO to USB  
* Insert the USB stick (8 GB or larger).  
* Open your chosen tool (Fedora Media Writer, Rufus, Etcher)  
* Select the downloaded ISO and choose the USB device as the target.  
* Start the write process and then eject the drive once the process is completed.  

### 4.3 Verifying bootability  
* Reboot your system and enter the firmware (BIOS/UEFI) boot menu (typically by pressing
F2/F10/Esc/F12).  
* Select the USB drive.  
* If you see the “Fedora” installer menu, you are ready to proceed.  

## 5 Booting the Installer  
* Boot from the USB drive under UEFI mode (recommended).  
* At the boot menu, select **Test this media and Start Fedora-Workstation-Live** and press
Enter.  
* The Fedora Installer will start.  

## 6 Installation Summary & Configuration  
### 6.1 Keyboard  
In the language page, you will also be able to change the keyboard layout if you want.  

### 6.2 Destination  
* Now, you will have to select the drive where you want to install the system.  
* It will consist of three options. These options will help in determining whether you
want to dual-boot the system or use the entire drive.  
* Lastly, you can also select the option of mount point assignment. This way, you will be able
to assign partitions to mount points.  

### 6.3 Encryption  
Now, the next option will be to select encryption. You may ignore this step.  

### 6.4 Confirmation  
* This page will give you a recap of the options that you have selected in the installation process.  
* You can finally select the erase data and install after the careful analysis of each selection.  

### 6.5 Installing Page 
* After the entire process is complete, you will be able to see the successful installation page.  
* You can select the “Exit to Live Desktop” option.  

## 7 First‑Boot Setup  
### 7.1 Welcome  
You can change the language of the system.  

### 7.2 Network 
Here, you can select the network to connect to the internet.  

### 7.3 Privacy  
You need to select the option to enable location services and problem reporting.  

### 7.4 Time Zone 
Next, you have the option to select the time zone.  

### 7.5 Repositories  
It gives you the option to enable third-party repositories.  

### 7.6 User Creation  
Finally, you need to set the login details. You can also go for enterprise login.  

### 7.7 Avatar Selection
Now, you can select the profile picture for your login account.  

### 7.8 Set Password
Lastly, you can set up a password for the Digital Scriptorium.  

### 7.9 Finish Installation
Click on "**Next**" and select **Start using Fedora Linux**.  
