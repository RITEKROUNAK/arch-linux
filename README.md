# Arch Linux
Installation Guide for Arch Linux

## Step 1: Download the Arch Linux ISO
   Download the ISO from the [Arch Linux download page](https://archlinux.org/download/).

## Step 2: Create a Live USB or Burn Arch Linux ISO to a DVD
   Once you have the Arch Linux ISO, you can create a live USB or burn it to a DVD.

   Create a Live USB of Arch Linux. Use a tool like [Rufus](https://rufus.ie/en/)
   
## Step 3: Boot up Arch Linux
   1. With the Arch Linux ISO burned on a DVD or stored as a live USB, insert the installation media into your computer and restart.

   2. Depending on your system, pressing F2, F10, or F12 lets you choose the device the system boots from.

   3. With the boot settings open, select the preferred install media (live USB or DVD). The following screen shows up after Arch Linux boots:

   ![VirtualBox_Arch Linux_17_08_2021_10_21_43](https://user-images.githubusercontent.com/64047505/129665623-107ec19c-b4ce-412f-99ca-fa32feb19e8a.png)
   
   4. Select Boot Arch Linux (x86_64, BIOS) and press Enter to start the setup process.
  
## Step 5: Check Your Internet Connection
   Check your Internet connection using the ping command:

    ping -c 3 google.com
    
   If you want to install Arch Linux using a wireless Internet connection, consult the [Arch Linux wiki’s wireless network configuration section](https://wiki.archlinux.org/title/Network_configuration/Wireless).
   
## Step 6: Enable Network Time Protocols (NTP)
   Next, enable Network Time Protocols (NTP) and allow the system to update the time via the Internet:

    timedatectl set-ntp true

   To check the NTP service status, use:

    timedatectl status
    
## Step 7: Partition the Disks
   1. Use the fdisk command to list all available disk drives:

    fdisk -l
   2. Find the name of the disk you want to partition. The name is displayed in the /dev/sdX format, where X is the drive letter.
   
   ![VirtualBox_Arch Linux_17_08_2021_10_28_00](https://user-images.githubusercontent.com/64047505/129666137-4ce426d0-ed9f-40d9-b386-63144a663360.png)

