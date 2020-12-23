# NiceHash OS local access
This guide provides information on how to configure log files to be persisted to NiceHash OS flash drive.

## NiceHash OS configuration
If you need additional information on how NiceHash OS configuration file looks like and how to modify it, please take a look at the [How to configure NiceHash OS](nhos_configuration.md) page.

## Configure og files persistance
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
