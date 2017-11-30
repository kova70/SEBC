```
[root@rodonode1 ~]# curl -X POST -u rodo-dev:cloudera 'http://localhost:7180/api/v1/clusters/Rodo-dev/services/hive/commands/stop'
{
  "id" : 981,
  "name" : "Stop",
  "startTime" : "2017-11-30T18:38:17.977Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }
}[root@rodonode1 ~]#curl -u rodo-dev:cloudera 'http://localhost:7180/api/v1/commands/981'
{
  "id" : 981,
  "name" : "Stop",
  "startTime" : "2017-11-30T18:38:17.977Z",
  "endTime" : "2017-11-30T18:38:19.895Z",
  "active" : false,
  "success" : true,
  "resultMessage" : "Successfully stopped service.",
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  },
  "children" : {
    "items" : [ {
      "id" : 982,
      "name" : "Stop",
      "startTime" : "2017-11-30T18:38:17.985Z",
      "endTime" : "2017-11-30T18:38:19.895Z",
      "active" : false,
      "success" : true,
      "resultMessage" : "Successfully stopped process.",
      "serviceRef" : {
        "clusterName" : "cluster",
        "serviceName" : "hive"
      },
      "roleRef" : {
        "clusterName" : "cluster",
        "serviceName" : "hive",
        "roleName" : "hive-HIVESERVER2-bf454a659df03992cc83e171281f78c2"
      }
    }, {
      "id" : 983,
      "name" : "Stop",
      "startTime" : "2017-11-30T18:38:17.988Z",
      "endTime" : "2017-11-30T18:38:19.882Z",
      "active" : false,
      "success" : true,
      "resultMessage" : "Successfully stopped process.",
      "serviceRef" : {
        "clusterName" : "cluster",
        "serviceName" : "hive"
      },
      "roleRef" : {
        "clusterName" : "cluster",
        "serviceName" : "hive",
        "roleName" : "hive-HIVEMETASTORE-bf454a659df03992cc83e171281f78c2"
      }
    } ]
  }
}[root@rodonode1 ~]# curl X POST -u rodo-dev:cloudera 'http://localhost:7180/api/v1/clusters/Rodo-dev/services/hive/commands/start'
{
  "id" : 987,
  "name" : "Start",
  "startTime" : "2017-11-30T18:39:58.856Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }
}
```
