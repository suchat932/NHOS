# NiceHash OS (beta)
NiceHash OS is a minimal standalone [Linux](https://en.wikipedia.org/wiki/Linux "Linux") operating system containing everything you need to start your own mining adventure.

## Quick setup guide
If you are familiar with the NiceHash OS you know already how thing are done.
Just as a reminder, here is al ist of steps you need to take to get going.
* Download NiceHash OS image from the following address https://nhos-test.nicehash.com/latest/package.
* Flash downloaded NiceHash OS image to the USB flash drive.
* Update NiceHash OS configuration file with your data.
<br/><br/>
## Slow setup guide
### Prerequisites
Even though there are no special prerequisites required to start using NiceHash OS, you will have to poses some basic technical skills and be familiar with operating system installed on your computer.

### Concepts
NiceHash OS is an operating system which loads from USB flash drive and runs from computer memory. It contains all the tools and drivers needed to bring your mining machine to life.

NiceHash OS flash drive is divided into two partitions, `SYSTEM` and `NHOS`. `SYSTEM` partition contains bootloader, Linux kernel and [RAM](https://en.wikipedia.org/wiki/Random-access_memory "Random Access Memory") file system, while `NHOS` partition contains NiceHash OS configuration file.

### Creating NiceHash OS flash drive
There are two steps in creating fully functional NiceHash OS flash drive
* Step one is to create USB flash drive containing an operating system. More detail description on how this is done is available on [How to create NiceHash OS flash drive](nhos_create_flash_drive.md) page.
* Step two is to update NiceHash OS configuration file with your data. More detail on which data you need to provide and where these should go is available on [How to configure NiceHash OS](nhos_configuration.md) page.

**Note**<br/>
This is a guide on how to prepare **one** NiceHash OS flash drive. If you plan to use the same setup on **multiple** machines then you can do the following. Go through the same steps as many times as how many NiceHash OS flash drives you need. After this you will end up with a bunch of NiceHash OS flash drives which contain **invalid** (empty) configuration. Now use **valid** configuration from your initial NiceHash OS flash drive and copy it to all newly created NiceHash OS drives.
<br/><br/>
## Finish
At this point you should have everything prepared to start using NiceHash OS. All you need to do now is to plug in NiceHash OS flash drive in to your mining machine and turn it on!

**Note**<br/>
Information on how to access mining machine locally is available on [NiceHash OS local access](nhos_local_access.md) page.
