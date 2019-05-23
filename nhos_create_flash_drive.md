# How to create NiceHash OS bootable flash drive
This guide provides information on how to create bootable flash drive with NiceHash OS. Following the instructions below, you will **download NiceHash OS image** (an `.img.gz` file), and then use **special application that writes an image to a USB drive**. You cannot simply copy the image file to a USB drive, you must use special software to write it properly.

## Prerequisites
* A computer connected to the internet with a **Windows**, **macOs** or **Linux** operating system.
* USB flash drive with **at least 2 GB** of space.
* You have a **special software to write image file to USB flash drive**.

**Note**<br/>
For creating NiceHash OS flash drive, you will need elevated privileges on your system (administrator privileges on Windows and root privileges on macOS or Linux).

**Warning**<br/>
The process described below will delete any data currently on your flash drive. Make sure to back up your flash drive's data to another storage location before proceeding.

## Install software for writing to USB flash drive
There are many tools available for writing image files to USB drive.
[**Ethcher**](https://etcher.io) is a example of a easy to use, cross-platform image burning tool.

**Note**<br/>
On systems like macOS and Linux users can also use command line tool `dd` to write image files to USB drive.

## Download NiceHash OS image
You can get **the latest NiceHash OS image** from our website.

## Write NiceHash OS image to USB drive
You can **write NiceHash image to USB drive** using aforementioned [**Ethcher**](https://etcher.io) tool. This tool can digest allot of different file formats. There is no need to decompress NiceHash OS image file beforehand.

There are three simple steps to write an image file using Etcher
1. Select NiceHash OS image file
2. Select USB drive to write an image file to
3. Start image writing process

![](graphics/etcher.gif)

**Note**<br/>
If you prefer to use command line tools instead, there are three simple steps to write an image file using `dd` tool
1. Decompress NiceHash OS image file<br/>
   `gunzip nhos-x.x.x.img.gz`
2. Define output device to write an image file to<br/>
   `/dev/sdax`
3. Start image writing process<br/>
   `dd if=nhos-x.x.x.img of=//dev/sdaX bs=4m && sync`

**Warning**<br/>
Be careful defining output device, wrong usage of `dd` tool can lead to **irreversible damage to your system**!
