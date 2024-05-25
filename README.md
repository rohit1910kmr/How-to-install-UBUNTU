# How-to-install-UBUNTU

# Install Ubuntu Desktop

## Overview

### What you’ll learn
In this tutorial, we will guide you through the steps required to install Ubuntu Desktop on your laptop or PC.

### What you’ll need
- A laptop or PC with at least 25GB of storage space.
- A flash drive (12GB or above recommended).
- If you are installing Ubuntu on a PC or laptop you have used previously, it is always recommended to back up your data before installation.

## 1. Download an Ubuntu Image

You can download an Ubuntu image [here](https://ubuntu.com/download/desktop). Make sure to save it to a memorable location on your PC! For this tutorial, we will use the Ubuntu 23.04 release, which uses the new Ubuntu Desktop installer that will be included in all future Ubuntu releases.

If you are installing an older version of Ubuntu, such as Ubuntu 22.04 LTS, you will find that the visual presentation of the installer is different, but the overall flow should remain the same.

## 2. Create a Bootable USB Stick

To install Ubuntu Desktop, write your downloaded ISO to a USB stick to create the installation media. This is not the same as copying the ISO and requires some bespoke software. For this tutorial, we’ll use [balenaEtcher](https://www.balena.io/etcher/), as it runs on Linux, Windows, and Mac OS. Choose the version that corresponds to your current operating system, and download and install the tool.

Select your downloaded ISO, choose your USB flash drive, and then click Flash! to install your image.

## 3. Boot from a USB Flash Drive

Insert the USB flash drive into the laptop or PC you want to use to install Ubuntu and boot or restart the device. It should recognize the installation media automatically. If not, try holding F12 during startup and selecting the USB device from the system-specific boot menu.

F12 is the most common key for bringing up your system’s boot menu, but Escape, F2, and F10 are common alternatives. If you’re unsure, look for a brief message when your system starts – this will often inform you of which key to press to bring up the boot menu.

Once the installer has initialized, you will be invited to choose your language and then presented with the option to try or install Ubuntu.

- If you click Try Ubuntu, you can preview Ubuntu without making any changes to your PC. You can return to the installer menu at any time by clicking the Install Ubuntu shortcut on the desktop.
- To proceed, click Install Ubuntu. You will be asked to select your keyboard layout. Once you’ve chosen one, click Continue.

Next, you will be asked to connect to Wi-Fi. This will allow Ubuntu to download updates and third-party drivers (such as NVIDIA graphics drivers) during installation. Once you have connected to Wi-Fi (or chosen to proceed offline), then we can continue to the installation setup.

**Alert: RST is enabled**  
Some PCs use Intel RST (Rapid Storage Technology), which is not supported by Ubuntu. If this is the case, then you will not be able to proceed beyond this point without disabling RST in the BIOS menu of your machine. If you encounter this pop-up, please visit [help.ubuntu.com/rst](https://help.ubuntu.com/rst) for more information.

## 4. Installation Setup

You will be prompted to choose between the Normal installation and Minimal installation options. The minimal installation is useful for those with smaller hard drives or who don’t require as many pre-installed applications.

In Other options, you will be prompted to download updates as well as third-party software that may improve device support and performance (for example, Nvidia graphics drivers) during the installation. It is recommended to check both of these boxes.

## 5. Type of Installation

This screen allows you to configure your installation. If you would like Ubuntu to be the only operating system on your hard drive, select Erase disk and install Ubuntu.

If your device currently has another operating system installed, you will receive additional options to install Ubuntu alongside that OS rather than replacing it.

### Installing Ubuntu alongside another operating system
If you select this option, you will be given a simple interface that allows you to select the drive you want to install Ubuntu on and a slider to determine the amount of disk space you would like Ubuntu to use. The available space is limited by the existing contents of the disk and is designed to avoid overwriting existing files.

This view automatically selects the largest partition on the drive. For more fine-grained control, you can switch to the Manual partitioning option that is detailed further down.

### Erase the disk and install Ubuntu
If you select this option, Ubuntu will take up the entire disk space on the selected drive.

If your PC has multiple hard drives, then this option allows you to install Ubuntu alongside an existing OS as long as they each have their drive. Take care to ensure that you are selecting the right drive in this instance!

This option also allows you to encrypt your entire drive using LVM. To do this, open the Advanced features option before proceeding to the above screen and select ‘Encrypt the new Ubuntu installation for security’.

LVM stands for Logical Volume Management. By using LVM during the setup, it makes it easier to create and manage partitions post-installation.

In the following step, you will be prompted to create a Security key that you will need to enter on boot before logging in with your user credentials.

**Note**: If you select encryption, you mustn't lose your security key! Write it down and store it in a safe place outside of your local system. You will not be
