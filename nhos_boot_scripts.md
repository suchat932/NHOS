# NiceHash OS boot scripts
This guide provides information on how to setup user provided shell scripts that NiceHash OS will execute on boot.

## What you will need
Here is the list of preconditions that must be met before you can proceed
* Computer with one of the following operating system: **Windows**, **MacOs** or **Linux**.
* **NiceHash OS flash drive**.
* **Text editor** you are familiar with.<br/>

## NiceHash OS configuration
NiceHash OS flash drive is divided into two partitions, **`SYSTEM`** and **`NHOS`**, where `NHOS` partition contains the configuration data for system to operate correctly.

When NiceHash OS flash drive is inserted into your computer, the system should **automatically detect `NHOS`** partition and **show it in system file manager** (Windows Explorer, macOS Finder, Linux Nautilus, etc.) as disk on Windows or as a mounted device on macOS and Linux. Using your file manager, navigate to the **location of the `NHOS` disk or mount point**. There you will find a **single configuration file** named **`configuration.txt`**.

## NiceHash OS boot scripts setup
When setting up NiceHash boot scripts for the first time, you should create a folder where user provided shell scripts are expected to reside. This folder must be located on the root of the **`NHOS`** partition (alongside  **`configuration.txt`**) and the name of this folder is expected to be **`scripts.sh`**. Inside this folder you can put one or many shell script files containing any commands that you wish to be executed at NiceHash OS boot. As long as this user provided shell script files names end with the **`*.sh`** extension, system will execute them. When script is executed, any console output from the script itself is persisted in the file at the same location and with the same name, but with an extension **`*.log`**.

#### Example
Create a shell script file ```example.sh``` with the following content
```sh
#!/bin/sh
echo "Hello world!"
```

Put this file into the expected location
\
```{NHOS}/scripts.sh/example.sh```

On NiceHash OS boot you should see the console output of the executed script in the script associated log file
\
```{NHOS}/scripts.sh/example.log```
