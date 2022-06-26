# Restore root password

It can be preliminary task for starting Your exam. It is crucial to know this procedure by heart. 

### Question:
 You do not know the root password but You have physical access to the machine. Create new root password
and log into the system.

***
(scroll down for an answer)

<br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/>
<br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/>





### Answer
#### [Cent8](https://linuxhint.com/reset-root-password-centos-8/)

1. Reboot into Grub menu, press 'e' to edit

2. Locate "ro" kernel parameter and replace it with "rw init=/sysroot/bin/sh"

3. Ctrl + X to enter ["single-user mode"](https://www.linuxtechi.com/boot-centos-8-rhel-8-single-user-mode/)

4. Mount root file system and reset root password by: 
```
chroot /sysroot
passwd root
```
