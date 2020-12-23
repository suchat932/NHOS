# NiceHash OS update configuration
This guide provides information on how to disable NiceHash OS automatic update.

## NiceHash OS configuration
If you need additional information on how NiceHash OS configuration file looks like and how to modify it, please take a look at the [How to configure NiceHash OS](nhos_configuration.md) page.

## Disable NiceHash OS automatic update
By default NiceHash OS will periodically check for an updates and execute an automatic update when one is available. Sometimes this behavior is not desired and user might want to disable automatic updates. To do this you must add the `update` section to JSON configuration file.

Example on how to disable NiceHash OS update
```json
{
    "rig": {
        "btc": "",
        "worker": "",
        "group": "",
    },
    "update": {
        "auto": false
    }
}
```

Beware that by disabling NiceHash OS from updating automatically you will have to execute update manually to update your system.

To manually execute system update just run the following command in the NiceHash OS mining rig command shell
```sh
sudo /opt/nhos/nhos_update
```