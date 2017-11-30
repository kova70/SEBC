# 1. Check vm.swappiness on all your nodes 
  `$ sysctl -a | grep vm.swappiness`<br>
  vm.swappiness = 30
  - Set the value to 1 <br>
    `$ sudo sysctl -w vm.swappiness=1`<br>
  vm.swappiness = 1 
  - Change the value in sysctl.conf <br>
  `$ sudo vi /etc/sysctl.conf`<br>
  vm.swappiness = 1
# 2. Show the mount attributes of your volume(s)
  `mount -l | grep '/sd'`<br>
  /dev/sda2 on / type xfs (rw,relatime,seclabel,attr2,inode64,noquota)<br>
  /dev/sda1 on /boot type xfs (rw,relatime,seclabel,attr2,inode64,noquota)<br>
  /dev/sdb1 on /mnt/resource type ext4 (rw,relatime,seclabel,data=ordered)<br>
  /dev/sdd1 on /disk4 type ext4 (rw,relatime,seclabel,data=ordered)<br>
  /dev/sdc1 on /opt type ext4 (rw,relatime,seclabel,data=ordered)<br>
