# SysmonBox

`SysmonBox` is a free sandbox framework based on [Microsoft Sysmon](https://docs.microsoft.com/en-us/sysinternals/downloads/sysmon). It can be used to run malware samples or any desired file in an isolated environment and get the behavior report. Sysmon can log a lot of information about sample's activity such as processes creation, network connections, registry changes and many others. 

```
=====================================================================
   ____                           ____             ____
  / __/_ _____ __ _  ___  ___    / __/__ ____  ___/ / /  ___ __ __
 _\ \/ // /_ -/  ' \/ _ \/ _ \  _\ \/ _ `/ _ \/ _  / _ \/ _ \\ \ /
/___/\_  /___/_/_/_/\___/_//_/ /___/\_,_/_//_/\_,_/_.__/\___//_\_\
    /___/
=====================================================================
Author: @n0dec
Site: https://github.com/n0dec/SysmonBox

[>] Restoring sysmonbox-initial snapshot
[>] Starting sandbox VM
[>] Copying file c:\projects\sysmonbox\sample.cmd to C:\Users\IEUser\Desktop\sample.cmd
[>] Clearing EventLog
[>] Executing sample C:\Users\IEUser\Desktop\sample.cmd
[>] Exporting sandbox report to reports\sample.cmd.text
[>] Powering off sandbox VM
```

## Usage
```commandline
> python sysmonbox.py --sample <sample file>
```

## Configuration
Before start running samples you will need a VM with Sysmon working on it. These are the steps to configure it in an simple way:

* [Install initial image](https://github.com/n0dec/SysmonBox/blob/master/INSTALL.md)
* [Configure the sandbox](https://github.com/n0dec/SysmonBox/blob/master/CONFIGURE.md)

### Executing sample
![sandbox](https://raw.githubusercontent.com/n0dec/SysmonBox/master/doc/4.png)
