$ echo never > /sys/kernel/mm/transparent_hugepage/defrag
$ echo never > /sys/kernel/mm/transparent_hugepage/enabled
$ chmod u+x /etc/rc.d/rc.local
$ vi /etc/rc.d/rc.local
systemctl start rc-local
systemctl enable rc-local
$ systemctl stop firewalld.service
$ systemctl disable firewalld.service
$ sysctl -a | grep vm.swappiness
vm.swappiness = 30
$ sudo sysctl -w vm.swappiness=1
vm.swappiness = 1
$ sudo vi /etc/sysctl.conf
$ sudo sysctl -p 
vm.swappiness = 1
$sudo fdisk -l
$sudo fdisk /dev/sdd
$sudo mkfs -t ext4 /dev/sdd1
$sudo more /etc/fstab
$sudo grep -i HugePages_Total /proc/meminfo
HugePages_Total:       0
$ifconfig
$getent hosts 10.2.0.4
10.2.0.4        rodonode1
$getent hosts 10.2.0.5
10.2.0.5        rodonode2
$ sudo yum install ntp
$ sudo systemctl start ntpd
$ sudo systemctl status ntpd
   Active: active (running) since Mon 2017-11-27 20:35:04 UTC; 2s ago
$ sudo yum update
$ sudo yum clean all
$ sudo mkdir /disk4
$ sudo mount /dev/sdc1 /disk4
$ sudo -i blkid
$ sudo more /etc/fstab
See man pages fstab(5), findfs(8), mount(8) and/or blkid(8) for more info
#
UUID=a36ed0da-7eb0-466f-8fb3-6d825ca254db /                       xfs     defaults        0 0
UUID=c27e9f73-821d-459e-a8b5-a8042fdc7461 /boot                   xfs     defaults        0 0
UUID=3d075e63-2b1e-4ff4-bf9f-a022923f55db /opt                    ext4    defaults        0 0
UUID=588418e3-9ecc-44a5-8501-802e3eed4df9 /disk4                  ext4    defaults        0 0
$ wget https://dev.mysql.com/get/mysql57-community-release-el7-11.noarch.rpm
$ wget http://archive.cloudera.com/cm5/redhat/7/x86_64/cm/5.12.0/RPMS/x86_64/jdk-6u31-linux-amd64.rpm
$ wget http://archive.cloudera.com/cm5/redhat/7/x86_64/cm/5.12.0/RPMS/x86_64/oracle-j2sdk1.7-1.7.0+update67-1.x86_64.rpm
$ sudo yum install ./jdk-6u31-linux-amd64.rpm
$ sudo yum install ./oracle-j2sdk1.7-1.7.0+update67-1.x86_64.rpm
$ sudo yum install ./mysql57-community-release-el7-11.noarch.rpm 
$ sudo yum install mysql-server
$ wget https://dev.mysql.com/get/Downloads/Connector-J/mysql-connector-java-5.1.44.zip
$ sudo systemctl start mysqld.service
$ grep "temporary password" /var/log/mysqld.log
2017-11-27T21:46:15.481569Z 1 [Note] A temporary password is generated for root@localhost: CeU+aCsOF8C!
$ sudo /usr/bin/mysql_secure_installation
$ sudo systemctl restart mysqld.service 
$ sudo vi cloudera-manager.repo
$ sudo mv cloudera-manager.repo /etc/yum.repos.d/
$ export CLASSPATH=/home/cloudera/mysql-connector-java-5.1.44/mysql-connector-java-5.1.44-bin.jar:$CLASSPATH
$ sudo cp mysql-connector-java-5.1.44/mysql-connector-java-5.1.44-bin.jar /usr/share/java/mysql-connector-java.jar
$ sudo yum install cloudera-manager-daemons cloudera-manager-server
$ sudo yum install cloudera-manager-agent
$ more /etc/my.cnf
$ sudo mv mysql-connector-java-5.1.44-bin.jar mysql-connector-java.jar
# vi /etc/cloudera-scm-server/db.properties
AGENTES
wget https://dev.mysql.com/get/mysql57-community-release-el7-11.noarch.rpm
yum install ./mysql57-community-release-el7-11.noarch.rpm
yum install mysql
wget https://dev.mysql.com/get/Downloads/Connector-J/mysql-connector-java-5.1.44.zip
unzip mysql-connector-java-5.1.44.zip
mkdir /usr/share/java
cp mysql-connector-java-5.1.44/mysql-connector-java-5.1.44-bin.jar /usr/share/java/mysql-connector-java.jar
ls -l /usr/share/java/
passwd root
DB
GRANT ALL PRIVILEGES ON oozie.* TO 'cloudera'@'localhost' identified by 'CapaCuatro1.';
GRANT ALL PRIVILEGES ON oozie.* TO 'cloudera'@'%' identified by 'CapaCuatro1.';
FLUSH PRIVILEGES;
Zookeeper
$ls -l /var/lib/
$mkdir /var/lib/zookeeper/version-2
$chown -R zookeeper:root /var/lib/zookeeper
$chmod 755 /var/lib/zookeeper
