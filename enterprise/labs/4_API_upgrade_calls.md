```
## Report the latest available version of the API
[root@rodonode1 ~]#  curl -u rodo-dev:cloudera 'http://localhost:7180/api/version'
v18
## Report the CM version
v18[root@rodonode1 ~]#  curl -u rodo-dev:cloudera 'http://localhost:7180/api/v18/cm/version'
{
  "version" : "5.13.0",
  "buildUser" : "jenkins",
  "buildTimestamp" : "20171002-1719",
  "gitHash" : "bd657e597e6743c458ee2c9aabe808b7c972981c",
  "snapshot" : false
## List all CM users  
}[root@rodonode1 ~]#  curl -u rodo-dev:cloudera 'http://localhost:7180/api/v18/users'
{
  "items" : [ {
    "name" : "admin",
    "roles" : [ "ROLE_LIMITED" ]
  }, {
    "name" : "minotaur",
    "roles" : [ "ROLE_CONFIGURATOR" ]
  }, {
    "name" : "rodo-dev",
    "roles" : [ "ROLE_ADMIN" ]
  } ]
  
 ## Report the database server in use by CM
 }[root@rodonode1 ~]#  curl -u rodo-dev:cloudera 'http://localhost:7180/api/v18/cm/scmDbInfo'
{
  "scmDbType" : "MYSQL",
  "embeddedDbUsed" : false
}
```
