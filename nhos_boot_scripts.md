# NiceHash OS boot scripts
This guide provides information on how to setup user provided shell scripts that NiceHash OS will execute on boot.

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
