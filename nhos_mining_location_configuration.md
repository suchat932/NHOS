# NiceHash OS mining location configuration
This guide provides information on how to configure NiceHash OS mining location.

## What you will need
Here is the list of preconditions that must be met before you can proceed
* Computer with one of the following operating system: **Windows**, **MacOs** or **Linux**.
* **NiceHash OS flash drive**.
* **Text editor** you are familiar with.<br/>

## NiceHash OS configuration
By default mining market location is selected automatically depending on the network conditions towards NiceHash servers. This behavior can be overridden via configuration where it is possible to specify preferred mining location.

NiceHash OS flash drive is divided into two partitions, **`SYSTEM`** and **`NHOS`**, where `NHOS` partition contains the configuration data for system to operate correctly.

When NiceHash OS flash drive is inserted into your computer, the system should **automatically detect `NHOS`** partition and **show it in system file manager** (Windows Explorer, macOS Finder, Linux Nautilus, etc.) as disk on Windows or as a mounted device on macOS and Linux. Using your file manager, navigate to the **location of the `NHOS` disk or mount point**. There you will find a **single configuration file** named **`configuration.txt`**.

To modify NiceHash OS configuration, open this configuration file with your preferred file editor where you will see the following file content structure
```json
{
    "rig": {
        "btc": "",
        "worker": "",
        "group": ""
    }
}
```

### Configure mining location
To configure mining location you must add the `location` option to the `rig` section in the JSON configuration file. Location configuration option can have one of two values, **`"eu"`** for Europe and **`"usa"`** for America. If no location option is specified, Europe is used as default.

Example on how to configure America as your mining location can be seen below
```json
{
    "rig": {
        "btc": "",
        "worker": "",
        "group": "",
        "location": "usa"
    }
}
```
