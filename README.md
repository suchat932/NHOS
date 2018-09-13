# NiceHash OS
NiceHash OS is a minimal standalone [Linux](https://en.wikipedia.org/wiki/Linux "Linux") operating system containing everything you need to start your own mining adventure.

## Download NiceHash OS image
If you are already familiar with the NiceHash OS flash drive creation, you can skip the rest of the page and just download the latest NiceHash OS image using the following address https://nhos-test.nicehash.com/latest/package.

## Prerequisites
Even though there are no special prerequisites required to start using NiceHash OS, you will have to poses some basic technical skills and be familiar with operating system installed on your computer.

## Concepts
NiceHash OS is an operating system which starts from USB flash drive where system is completely loaded into computer memory. It contains all the tools and drivers needed to bring your mining machine to life.

NiceHash OS flash drive is divided into two partitions, `SYSTEM` and `NHOS`. `SYSTEM` partition contains bootloader, Linux kernel and [RAM](https://en.wikipedia.org/wiki/Random-access_memory "Random Access Memory") file system, while `NHOS` partition contains configuration data user needs to provide for system to work correctly.

## Creating NiceHash OS flash drive
There are two steps in creating fully functional NiceHash OS flash drive
* Step one is to create USB flash drive containing an operating system. More detail description on how this is done is available on [How to create NiceHash OS flash drive](nhos_create_flash_drive.md) page.
* Step two is to provide all configuration data for system to work correctly. More detail on which data you need to provide and where these should be located is available on [How to configure NiceHash OS](nhos_configuration.md) page.

**Note**<br/>
The procedure described above is a guide to prepare **one** NiceHash OS flash drive. If you plan to use the same setup on **multiple** machines then you can do the following. Go through the NiceHash OS flash drive creation steps as many times as how many NiceHash OS flash drives you need. After this step you will end up with a bunch of NiceHash OS flash drives which contain **invalid** (empty) configuration. Now use **valid** configuration from your initial NiceHash OS flash drive and copy it to all newly created NiceHash OS drives.

## Finish
At this point you should have everything prepared to start using NiceHash OS. All you need to do now is to plug in NiceHash OS flash drive into your mining machine and turn it on!
