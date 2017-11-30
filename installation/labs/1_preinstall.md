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
# 3. Disable transparent hugepage support
  If the value of HugePages_Total is "0" it means HugePages is disabled on the system.<br>
  `$sudo grep -i HugePages_Total /proc/meminfo`<br>
  HugePages_Total:       0 <br>
# 4. List your network interface configuration
  `ifconfig`<br>
  <br>eth0: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 1500
        inet 10.2.0.4  netmask 255.255.255.0  broadcast 10.2.0.255
        inet6 fe80::20d:3aff:fe32:982b  prefixlen 64  scopeid 0x20<link>
        ether 00:0d:3a:32:98:2b  txqueuelen 1000  (Ethernet)
        RX packets 11042531  bytes 8037007462 (7.4 GiB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 7053068  bytes 4398041175 (4.0 GiB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0<br>
# 5.Show that forward and reverse host lookups are correctly resolved
  `dig rodonode1`<br>
  ANSWER SECTION:<br>
  rodonode1.		0	IN	A	10.2.0.4<br>
  `dig -x 10.2.0.4`<br>
  ANSWER SECTION:<br>
  4.0.2.10.in-addr.arpa.	0	IN	PTR	rodonode1.rodo.com.<br>
 # 6.Show the nscd service is running
  `systemctl status nscd.service`
   <br>nscd.service - Name Service Cache Daemon
   Loaded: loaded (/usr/lib/systemd/system/nscd.service; disabled; vendor preset: disabled)
   Active: active (running) since Thu 2017-11-30 22:49:18 UTC; 4s ago<br>
 # 7. Show the ntpd service is running
  `systemctl status ntpd.service `
   <br>ntpd.service - Network Time Service
   Loaded: loaded (/usr/lib/systemd/system/ntpd.service; disabled; vendor preset: disabled)
   Active: active (running) since Wed 2017-11-29 21:34:11 UTC; 1 day 1h ago<br>
 
