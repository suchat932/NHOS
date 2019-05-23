# NiceHash OS bug reporting
This guide provides information on how to report a bug concerning NiceHash OS.

## Prerequisites
* Access to the **mining machine** with a **running NiceHash OS system**
* You are **familiar with a Linux shell** and how to access your mining machine locally or remotely.

## Bug reporting
If you believe that you've found a bug that should be reported to NiceHash, then make sure to **describe it as precise as possible**. But be sure to also send us **a copy of the NiceHash OS system dump** file, as this will be of great help to our developers.

There are two commands available which you can use to generate **NiceHash OS system dump** file.
* **`nhos_system_dump_save`** - will generate **system dump file** and **save it to the USB flash key**.
* **`nhos_system_dump_push`** - will generate **system dump file** and **push it to the NiceHash network storage**.

**Note**<br/>
If you are familiar with the Linux operating system then it should be fairly simple to retrieve system dump file from your mining machine. You can access your mining machine locally and then just copy the file to an external media or access your mining machine remotely using SFTP client (WinSCP, FileZilla, CyberDuck, etc.) and get the file this way.
