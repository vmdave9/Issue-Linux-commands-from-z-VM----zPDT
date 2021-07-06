**Issue-Linux-commands-from-z-VM----zPDT**

A short Rexx exec to issue host Linux commands from a z/VM image running on zPDT This is just a simple Rexx exec to issue host Linux commands from z/VM, using the zPDT device drive, awscmd.

To use it, just copy the Rexx exec to a CMS user id and add a device stanza like this:
```
[manager] 
name awscmd 20 
device 580 3480 3480
```

to the device map. That's it.

Output will look something like this:
```
oscmd ls d*
STDOUT output------
dave2.req
dave.req
dave.zip
desktop.ini
STDERR output ------
Ready; T=0.02/0.04 15:13:13
```
