Linux Setup Guide Outline
- This guide will cover setting up a basic Linux install on a Windows PC for the specific purpose of speedrunning and streaming Hollow Knight. Linux's more optimized filesystem and generally lower resource consumption tends to reduce load times and boost performance slightly. In Hollow Knight 1221 specifically it also drastically decreases the freeze frames from collecting any base-level spell (ie Vengeful Spirit).
- This guide is intended for those not looking to fully commit to Linux. Instead, we'll set up a dual-boot of Linux and Windows so you can just switch to Linux for runs.
- Since this guide expects no experience with Linux, we'll also go over some basics of navigating the operating system (such as using the software manager, some basic terminal commands, and how to look for help online)

You will need:
- USB flash drive
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
    - "Canonical" Ubuntu: The most widely used Linux distro. Has professional support teams and is extremely general-purpose, but can be a bit overwhelming and bloated for specific use-cases like ours
      - https://ubuntu.com/download/desktop
  - If you'd like to experiment with other types of Linux, Arch (SteamOS, Bazzite) and Fedora (Pop_OS!, Nobara) are other popular and well-supported choices

Linux Installation
- Install or plug in your second drive
	- If you don't have a second drive, you'll need to add a new partition to your main drive with enough space for Linux and all the apps + some space for recordings. I'd say no less than 64gb or even 128gb, but use what your resources allow
	- BACKUP YOUR DRIVE BEFORE PARTITIONING, especially if you've never done it. Partitioning and formatting drives can destroy the data on those drives if not done carefully
	- If the drive is external, plan to leave it plugged in whenever possible. Unplugging the drive while it's in use can corrupt the data on the drive or damage the drive itself.
- Download 
