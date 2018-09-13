# How to configure NiceHash OS
This guide provides information on how to configure NiceHash OS to work properly once flash drive has been created. If you do not have NiceHash OS flash drive created yet then jump to [How to create NiceHash OS flash drive](nhos_create_flash_drive.md) page for further instructions.


## What you will need
Here is the list of preconditions that must be met before you can proceed
* You have a **Windows**, **macOs** or **Linux** computer.
* You have a NiceHash OS flash drive.
* You have a text editor you are familiar with.<br/>

**Note**<br/>
Any text editor is fine as long as it does not mess up the file format being edited. Depending on the operating system you are using you might consider some of the following options

**Windows** - *Notepad*, [*Notepad++*](https://notepad-plus-plus.org/), [*PSPad*](http://www.pspad.com/), [*Atom*](https://atom.io/), [*Brackets*](http://brackets.io/), [*Visual Studio Code*](https://code.visualstudio.com/)<br/>
**macOS** - *TextEdit*, [*Atom*](https://atom.io/), [*Brackets*](http://brackets.io/), [*Visual Studio Code*](https://code.visualstudio.com/)<br/>
**Linux** - *vi*, [*nano*](https://www.nano-editor.org/), [*Geany*](https://www.geany.org/), [*KWrite*](https://www.kde.org/applications/utilities/kwrite/), [*Atom*](https://atom.io/), [*Brackets*](http://brackets.io/), [*Visual Studio Code*](https://code.visualstudio.com/)<br/>

## NiceHash OS configuration
NiceHash OS flash drive is divided into two partitions, `SYSTEM` and `NHOS` where `NHOS` partition contains configuration data for system to operate correctly. When NiceHas OS flash drive is inserted into your computer system should automatically detect `NHOS` partition and show it in system file manager (Windows Explorer, macOS Finder, Linux Nautilus, etc.) as disk on Windows or as a mounted device on macOS and Linux. Using your file manager, navigate to the location of the `NHOS` disk or mount point. There you will find a single configuration file named `configuration.txt`. 

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
Configuration is divided into different sections: **rig**, **access** and **network**. All the sections contain configuration entries which are named to be as self explanatory as possible.
 
### Rig
This section is used to configure NiceHas OS mining feature.<br/>

`btc` - Your NiceHash BTC address. &nbsp;&nbsp;[**mandatory**]<br/>
`worker` - Name your mining machine (also known as *Rig name*). &nbsp;&nbsp;[**optional**]<br/>
`group` - Put your mining machine into group. &nbsp;&nbsp;[**optional**]

### Access
This section is used to configure user access to the mining machine. For security reasons only SSH access is possible. If you want to have access to your mining machine you must fill in this section, otherwise leave it empty.<br/>

`ssh` - SSH public key for user authentication.

### Network
This section is used to configure the mining machine network settings. There are only wireless configuration entries here, and if you are using wireless infrastructure you must fill in this section, otherwise leave it empty.<br/>

`ssid` - [SSID](https://en.wikipedia.org/wiki/Service_set_(802.11_network)#Service_set_identifier_(SSID) "Service Set Identifier") to provide the name for a wireless network access.<br/>
`key` - Security key for wireless network access authentication.

**Note**<br/>
For security reasons only [WPA](https://en.wikipedia.org/wiki/Wi-Fi_Protected_Access "Wi-Fi Protected Access") and [WPA2](https://en.wikipedia.org/wiki/Wi-Fi_Protected_Access "Wi-Fi Protected Access 2") security protocols are supported. 

**Note**<br/>
There are no configuration entries to configure wired network setting. Also there are no configuration entries to define static IP address to be assigned to the mining machine. No matter if you are running the mining machine on a wired or wireless infrastructure, IP address is always assigned dynamically using [DHCP](https://en.wikipedia.org/wiki/Dynamic_Host_Configuration_Protocol "Dynamic Host Configuration Protocol") protocol.<br/><br/>

**Example on how configuration might look like after modification**
```json
{
    "rig": {
        "btc": "2N8xDN798uKMgPxTt35pgmGcdpJnSAvgsMF",
        "worker": "centaurus",
        "group": "constellation"
    },
    "access": {
        "ssh": {
            "key": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQCoWwJIm9JNgWzPrsMAeYWdM4nAkCET4j1kONsGPE2GeKul/4dTiq8X8aTKVdLLXOTQxBsOjb6J4umgVioTuorthjD0lYM3HDp55BnBgcnXXm7TfKzWKyCcbXvpOZA1pdzLKTo8bSBWjq4P2J0xPO6A6QHQvQs2LDPc5SyDMYrXOKrPLHfNxzxg9mvry49RtQJSzBICnBWDc28pNSCjvKbeHzEA85Quy4ctR7A7cHHeR0G3k/Xozdc8/eUptxhbW2M4t4uUg4Tnh4OQEPJKQ5j4zvkqRxrzMV1Kvxuarxbouwci569ulaOYDUQI0S8BB57d5IP3HRvsG4Ok8HosIxTJ"
        }
    },
    "network": {
        "wireless": {
            "ssid": "zodiac",
            "key": "8!Lf@I5s3tpY"
        }
    }
}
```
<br/>

When you are done with configuration modifications, save your changes and safely unplug NiceHash OS flash drive from your computer.
