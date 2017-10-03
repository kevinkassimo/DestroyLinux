# Ways to f**k up your Linux

### SUDO rm -rf /bin, /usr, /etc...
I've done once myself. Great fun.  
Also, according to Bumblebee, putting a *space* between `/usr` and `/...`, without quotes, is also thrilling!  
```
rm -rf /usr /... # huge WIN!
```
Even better, by Steam on Linux, a variable that evaluates to `""`!  
```
rm -rf "$EMPTYVAR/"
```

### Tampering with Runlevels  
Setting default runlevel to 0 (shutdown) and 6 (reboot). You'll stuck there.  
```bash
# in /etc/init/rc-sysinit.conf
env DEFAULT_RUNLEVEL=0 # or 6
```  

### Filesystem Table  
Try doing something else with your `/etc/fstab` and then reboot.  

### Moving /etc to Somewhere Else
How about a *new partition* away from `/`? Sounds like a good idea.  

### EFI, grub, ...
(Actually for Mac users, more often)  
What is that `EFI` partition? It is taking up some space. Can I just clear everything inside?  
And `/boot`...  
