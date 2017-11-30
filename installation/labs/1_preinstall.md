# Check vm.swappiness on all your nodes 

```$ sysctl -a | grep vm.swappiness```
vm.swappiness = 30
$ sudo sysctl -w vm.swappiness=1
vm.swappiness = 1
$ sudo vi /etc/sysctl.conf
