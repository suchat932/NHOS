# NiceHash OS local access
This guide provides information on how to configure log files to be persisted to NiceHash OS flash drive.

## What you will need
Here is the list of preconditions that must be met before you can proceed
* Computer with one of the following operating system: **Windows**, **MacOs** or **Linux**.
* **NiceHash OS flash drive**.
* **Text editor** you are familiar with.<br/>

## NiceHash OS configuration
NiceHash OS flash drive is divided into two partitions, **`SYSTEM`** and **`NHOS`**, where `NHOS` partition contains the configuration data for system to operate correctly.

When NiceHash OS flash drive is inserted into your computer, the system should **automatically detect `NHOS`** partition and **show it in system file manager** (Windows Explorer, macOS Finder, Linux Nautilus, etc.) as disk on Windows or as a mounted device on macOS and Linux. Using your file manager, navigate to the **location of the `NHOS` disk or mount point**. There you will find a **single configuration file** named **`configuration.txt`**.

To modify NiceHash OS configuration, open this configuration file with your preferred file editor where you will see the following file content structure
```json
{
    "rig": {
        "btc": "",
        "worker": "",
        "group": ""
    },
    "access": {
        "ssh": {
            "key": ""
        }
    },
    "network": {
        "wireless": {
            "ssid": "",
            "key": ""
        }
    }
}
```

To configure log files to be persisted to NiceHash OS flash drive you must add the log persistance setting to JSON configuration file as specified below
```json
{
    "rig": {
        "btc": "",
        "worker": "",
        "group": ""
    },
    "access": {
        "ssh": {
            "key": ""
        }
    },
    "network": {
        "wireless": {
            "ssid": "",
            "key": ""
        }
    },
    "log": {
        "persist": true
    }
}
```

**Warning**<br/>
Persisting log files to USB flash drive is meant to be used only for debugging purposes. Writing to USB flash drive for an extended period of time can lead to **irreversible damage to flash drive itself**!
