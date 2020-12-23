# NiceHash OS mining location configuration
This guide provides information on how to configure NiceHash OS mining location.

## NiceHash OS configuration
If you need additional information on how NiceHash OS configuration file looks like and how to modify it, please take a look at the [How to configure NiceHash OS](nhos_configuration.md) page.

## Configure mining location
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
