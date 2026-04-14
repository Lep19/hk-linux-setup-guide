Linux Setup Guide Outline
- This guide will cover setting up a basic Linux install on a Windows PC for the specific purpose of speedrunning and streaming Hollow Knight. Linux's more optimized filesystem and generally lower resource consumption tends to reduce load times and boost performance slightly. In Hollow Knight 1221 specifically it also drastically decreases the freeze frames from collecting any base-level spell (ie Vengeful Spirit).
- This guide is intended for those not looking to fully commit to Linux. Instead, we'll set up a dual-boot of Linux and Windows so you can just switch to Linux for runs.
- Since this guide expects no experience with Linux, we'll also go over some basics of navigating the operating system (such as using the software manager, some basic terminal commands, and how to look for help online)
- This can work with some minor changes on older Mac computers using x86 CPUs, however modern Macs use Apple's proprietary CPU architecture. Linux support for Apple silicon is limited at this time and is beyond the scope of this guide

You will need:
- USB flash drive (min. 8gb recommended)
- Non-bluetooth keyboard (a mouse can be nice too but isn't required)
  - We'll need to be able to control the computer before we're in an operating system, and bluetooth devices won't be able to connect during those times
- Technically optional but very recommended: a second hard drive/SSD. Internal will give you better reliability and speed, but external technically can work if it's all you have access to
	- Note the distinction between the flash drive and the second drive; we will use the flash drive temporarily to install Linux onto the second drive permanently
- Rufus
  - https://rufus.ie/en/
- A Linux image/ISO
  - I'd personally recommend an Ubuntu-based distro for their great compatibility and relative ease of use. Some examples:
    - Zorin OS: My personal favorite. Designed to be intuitive for Windows users, has a nice UI, generally supports gaming without much fuss, has dedicated forums for troubleshooting
      - https://zorin.com/os/download/
    - Linux Mint: The classic beginner Linux distro. Has a slightly dated UI but an abundance of resources for troubleshooting
      - https://linuxmint.com/download.php
    - "Canonical" Ubuntu: The most widely used Linux distro. Has professional support teams and is extremely general-purpose, but can be a bit overwhelming and bloated for more casual use-cases like ours
      - https://ubuntu.com/download/desktop
  - If you'd like to experiment with other types of Linux, Arch (SteamOS, Bazzite) and Fedora (Pop_OS!, Nobara) are other popular and well-supported choices

Linux Installation
- Install or plug in your second drive
	- If you don't have a second drive, you'll need to add a new partition to your main drive with enough space for Linux and all the apps + some space for recordings. I'd say no less than 64gb or even 128gb, but use what your resources allow
	- BACKUP YOUR DRIVE BEFORE PARTITIONING, especially if you've never done it. Partitioning and formatting drives can destroy the data on those drives if not done carefully
	- If the drive is external, plan to leave it plugged in whenever possible. Unplugging the drive while it's in use can corrupt the data on the drive or damage the drive itself.
- Plug in your flash drive
- Use Rufus and your Linux image to turn your flash drive into a bootable drive
  - In the Device dropdown, select your flash drive. If the name is unclear, use the capacity to determine which to pick
  - In the Boot selection dropdown, select Disk or ISO Image, click Browse, then navigate to and select your Linux image (should be a .iso file)
  - The rest of the default settings should be fine
  - When the READY bar lights up, click the START button at the bottom. Rufus should warn you of this, but this will wipe all data on that flash drive. Please back up anything important on it before clicking START
- Enter your computer's BIOS
  - Go to Settings -> System -> Recovery -> Advanced startup and click "Restart now," then choose Troubleshoot -> Advanced Options -> UEFI Firmware Settings
  - The exact layout of your BIOS will depend on your motherboard, but you'll want to find something relating to Boot or Boot Order, then change the order of the devices to put your flash drive at the top of the list. If you have a mouse, navigating should be pretty straightforward. If not, use the arrow keys and Enter on your keyboard to navigate between menus, and look for more specific controls on the BIOS screen itself
  - Save and Exit BIOS. Your computer should restart and boot into your Linux install image
- Follow the installer
  - Most modern installers are pretty self-explanatory. Just keep an eye out for where it's asking you to install to
    - If you're using a second drive, you may need to choose "Custom" or "Manual" to select the drive yourself. If you're not, look for "Install alongside my current OS" or something similar. Again, PLEASE backup your drive before doing this if you're not familiar with partitioning or disk management
    - Once you're finished, you'll be prompted to restart and remove your flash drive
