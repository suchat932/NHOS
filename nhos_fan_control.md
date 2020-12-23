# NiceHash OS fan control
This guide provides information on how to configure custom GPU fan control table.

## NiceHash OS configuration
If you need additional information on how NiceHash OS configuration file looks like and how to modify it, please take a look at the [How to configure NiceHash OS](nhos_configuration.md) page.

## Configure custom GPU fan curve
To configure your custom GPU fan control table you must add table values to JSON configuration file as specified below
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
    "fan_control": [
        {"tmpc": 40, "spdp" : 25},
        {"tmpc": 45, "spdp" : 35},
        {"tmpc": 50, "spdp" : 40},
        {"tmpc": 55, "spdp" : 50},
        {"tmpc": 60, "spdp" : 60},
        {"tmpc": 65, "spdp" : 70},
        {"tmpc": 70, "spdp" : 75},
        {"tmpc": 75, "spdp" : 80},
        {"tmpc": 80, "spdp" : 85},
        {"tmpc": 85, "spdp" : 95},
        {"tmpc": 90, "spdp" : 100}
    ]
}
```
From the example fan control table above one can see that table has two columns. First column specifies temperature in degrees celsius while second column specifies desired fan speed in percent when specified temperature is reached.
