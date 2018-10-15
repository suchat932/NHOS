# NiceHash OS local access
This guide provides information on how to report a bug concerning NiceHash OS.

## What you will need
Here is the list of preconditions that must be met before you can proceed
* You have access to the mining machine with a running NiceHash OS system
* You have a keyboard and monitor connected to the mining machine.
* You are familiar with Linux shell and how to access your mining machine locally or remotely.

## Bug reporting
If you believe that you've found a bug that should be reported to NiceHash, then make sure to describe it as precise as possible. It will be of great help to our developers team that you also attach NiceHash OS system **log** files.

System and application log files are located under `/var/log/nhos` directory.
* `boot.log` - contains information on NiceHash OS boot sequence
* `nhm.log` - contains information on NiceHash Miner operations
* `excavator.log` - contains information on NiceHash Miner mining service operations
* `update.log` - contains information on NiceHash OS update service operations

At the very least, you should attach `boot.log`, `nhm.log` and `excavator.log` files to your bug report.

**Note**<br/>
If you are familiar with the Linux operating system then it should be fairly simple task to retrieve log files from your mining machine. You can access your mining machine locally and then just copy the files to some external media or access your mining machine remotely using SFTP client (WinSCP, FileZilla, CyberDuck, etc.) and get the log files this way.
