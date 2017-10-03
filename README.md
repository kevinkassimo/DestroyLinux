# Ways to f**k up your Linux

### Tampering with Runlevels  
Setting default runlevel to 0 (shutdown) and 6 (reboot). You'll stuck there.  
```bash
# in /etc/init/rc-sysinit.conf
env DEFAULT_RUNLEVEL=0 # or 6
```  

### Filesystem Table  
Try doing something else with your `/etc/fstab` and then reboot.  

