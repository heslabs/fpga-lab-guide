### Create SD Card Image

* While some Linux systems only require a single FAT-formatted boot partition (e.g. those that use a ramdisk), some systems require a second ext4 formatted partition to hold the root filesystem.  
  * The FAT partition will be referred to as the "boot" partition, which is used to hold the boot image (BOOT.BIN) and Linux image (image.ub or Image + .dtb).  
  * The ext4 partition for the root filesystem will be referred to as "root". 

* These steps assume you're using a blank, unformatted SD card with no existing partitions on it. We'll use the fdisk utility in Linux to create the new partitions. 
fdisk is text based tool used to create partitions on a disk. 
You can also use gparted which is gui-base partitioning tool.

---
### Step to Create SD Card Image

1. Create two partitions

    * Unmount your disk and start fdisk with your device name. In my case my SD card is at /dev/sdc:

2. Formatting the Partitions
    * After creating the partitions, the next step is to format them with the appropriate files system. 

3. Copy the Images to the New Partitions
    * Mount the partitions so you can copy your boot images and root file system to the card. 

4. Unmount and eject the SD card from your Linux host

---
### SD Card Partition

The contents of this SDCard are illustrated as below

<img src="https://github.com/user-attachments/assets/6e2088b3-2ee7-4f60-bdcd-7f00cb272c19" width="700">

---
### Write Image into SD Card

* For setting up the microSD card, you’ll need to download the latest SD card image and then write it using an Image Flashing tool.
* Download the [Balena Etche](https://www.balena.io/etcher/) (recommended; available for Window, Linux, and macOS). Follow the instructions in the tool and select the downloaded image to flash onto your microSD card

<img src="https://github.com/user-attachments/assets/936ccbf7-ef21-4765-ba6a-eb6527d7376e" width="500">

---
### Free Windows Disk Image Write

* Free Windows Disk Image Writer: Create bootable USB drives
    * Win32DiskImager [https://win32diskimager.download ]
    * Balena Etcher [https://www.balena.io/etcher/] 
    * Rufus [https://rufus.ie/en_US]

<img src="https://github.com/user-attachments/assets/7a64cfd4-9de0-4c77-b870-075d4eab9844" width="800">



