# NiceHash OS local access
This guide provides information on how to **access NiceHash OS locally**.

## Prerequisites
* Access to the **mining machine** with a **running NiceHash OS system**
* **Keyboard and monitor connected** to the **mining machine**.

## How to log in to the system
On system start, you are presented with a screen where you can **enter access credentials to log in** to the system. There is only **one user configured for accessing NiceHash OS** and there is **no password required** to log in locally. Just **enter username `nhos`** and **hit _Enter_ key** (_Return_ on some systems).

**NiceHash OS is a minimal Linux operating system** based on [_Tiny Core Linux_](http://tinycorelinux.net). If you are familiar with any Linux distribution, then you will feel comfortable using NiceHash OS as well.

## Places to check out
**System configuration**<br/>
NiceHash OS configuration prepared while creating NiceHash OS flash drive is located under `/mnt/nhos` directory in `configuration.txt` file.

**System logs**<br/>
System startup and application logs are located under `/var/log/nhos` directory.
* `nhos_boot.log` - contains information on NiceHash OS boot sequence
* `nhos_nhm.log` - contains information on NiceHash Miner operations
* `nhos_update.log` - contains information on NiceHash OS update service operations

## System usage
There are **no special usage cases logging in to the NiceHash OS system** other than **checking system configuration** and **logs** in case something is not working as expected. Please remember that NiceHash OS is **running completely from computer memory** and **any changes** you might have done to the system are **lost on reboot**. The only location where changes are persisted are the ones under `/mnt/nhos` directory.
