# NiceHash OS local access
This guide provides information on how to access NiceHash OS locally.  create bootable flash drive with NiceHash OS. Following the instructions below, you will download NiceHash OS image (an `.img.gz` file), and then use special application that writes an image to a USB drive. You cannot simply copy the image file to a USB drive, you must use special software to write it properly.

## What you will need
Here is the list of preconditions that must be met before you can proceed
* You have access to the mining machine with a running NiceHash OS system
* You have a keyboard and monitor connected to the mining machine.

## How to log in to the system
On system start you are presented with a screen where you can enter access credentials to log in to the system. There is only one user configured for accessing NiceHash OS and there is no password required to log in locally. Just enter username `nhos` and hit _Enter_ key (_Return_ on some systems).

NiceHash OS is a minimal Linux operating system based on [Tiny Core Linux](http://tinycorelinux.net). If you are familiar with any Linux distribution, then you will feel comfortable using NiceHash OS as well.

## Places to check out
**System configuration**<br/>
NiceHash OS configuration prepared while creating NiceHash OS flash drive is located under `/mnt/nhos` directory in `configuration.txt` file.

**System logs**<br/>
System startup and application logs are located under `/var/log/nhos` directory.
* `boot.log` - contains information on NiceHash OS boot sequence
* `nhm.log` - contains information on NiceHash Miner operations
* `excavator.log` - contains information on NiceHash Miner mining service operations
* `update.log` - contains information on NiceHash OS update service operations

## System usage
There are no special usage cases logging in to the NiceHash OS system other than checking system configuration and logs in case something is not working as expected. Please remember that NiceHash OS is running completely from [RAM](https://en.wikipedia.org/wiki/Random-access_memory "Random Access Memory") and any changes you might have done to the system are lost on reboot. The only location where changes are persisted are the ones under `/mnt/nhos` directory.
