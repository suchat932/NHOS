# NiceHash OS
NiceHash OS is a minimal standalone [Linux](https://en.wikipedia.org/wiki/Linux "Linux") operating system containing everything you need to start mining crypto-currency efficiently.

## Quick setup guide
Below is a list of steps get NHOS up and running.
* **Download NiceHash OS image** from our website.
* **Flash downloaded NiceHash OS** image to the **USB flash drive**.
* Update NiceHash OS configuration file with your data.
<br/><br/>
## Detailed setup guide
### Prerequisites
There are no special prerequisites required to start using NiceHash OS.

### Concepts
NiceHash OS is an **operating system** which loads from **USB flash drive** and **runs from computer memory**. It contains **all the tools and drivers needed** to bring your mining machine to life.

NiceHash OS flash drive is divided into two partitions, **`SYSTEM`** and **`NHOS`**. `SYSTEM` partition contains bootloader, Linux kernel and [RAM](https://en.wikipedia.org/wiki/Random-access_memory "Random Access Memory") file system, while `NHOS` partition contains NiceHash OS configuration file.

### Creating NiceHash OS flash drive
There are two steps required to create a fully functional NiceHash OS flash drive
1) **Create a USB flash** drive **containing an operating system**. Detailed instructions are available on [How to create NiceHash OS flash drive](nhos_create_flash_drive.md) page.
2) **Update NiceHash OS configuration file with your data**. Detailed instructions are available on [How to configure NiceHash OS](nhos_configuration.md) page.

**Note**<br/>
This is a guide on how to prepare **one** NiceHash OS flash drive. If you plan to use the same setup on **multiple** machines then you can do the following. Go through the steps mentioned above for each NiceHash OS flash drives you need. After this, you will have multiple NiceHash OS flash drives which contain a **invalid** (empty) configuration. Now use **valid** configuration from your initial NiceHash OS flash drive and copy it to all newly created NiceHash OS drives.
<br/><br/>
## Finish
At this point you should have everything prepared to start using NiceHash OS. All you need to do now is to **plug in NiceHash OS flash drive in to your mining machine and turn it on!**

**Note**<br/>
Information on how to access mining machine locally is available on [NiceHash OS local access](nhos_local_access.md) page.

**Note**<br/>
Information on how to report bugs is available on [NiceHash OS bug reporting](nhos_bug_reporting.md) page.

**Note**<br/>
Information on how to customize fan control table is available on [NiceHash OS fan control](nhos_fan_control.md) page.

**Note**<br/>
Information on how to persist miner log files to USB flash drive is available on [NiceHash OS log persist](nhos_log_persist.md) page.

**Note**<br/>
Information on how to setup user provided shell scripts that are executed on system boot is available on [NiceHash OS boot scripts](nhos_boot_scripts.md) page.

**Note**<br/>
Advanced users who want to squeeze the last atom of power out of their graphics cards cant experiment with graphics cards overclocking. Beware that sometimes graphics cards overclocking can have a negative impact on system stability. Information on how this is done for NiceHash Miner is available on [Manual OC settings](nhos_manual_oc_settings.md) page.
