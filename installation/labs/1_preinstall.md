# 1. Check vm.swappiness on all your nodes 
  ```$ sysctl -a | grep vm.swappiness```
  vm.swappiness = 30
  - Set the value to 1 
    ```$ sudo sysctl -w vm.swappiness=1```
  vm.swappiness = 1
  - Change the value in sysctl.conf
  ```$ sudo vi /etc/sysctl.conf```
  vm.swappiness = 1
# 2. Show the mount attributes of your volume(s)
  ```mount -l | grep '/sd'```
  /dev/sda2 on / type xfs (rw,relatime,seclabel,attr2,inode64,noquota)
  /dev/sda1 on /boot type xfs (rw,relatime,seclabel,attr2,inode64,noquota)
  /dev/sdb1 on /mnt/resource type ext4 (rw,relatime,seclabel,data=ordered)
  /dev/sdd1 on /disk4 type ext4 (rw,relatime,seclabel,data=ordered)
  /dev/sdc1 on /opt type ext4 (rw,relatime,seclabel,data=ordered)
