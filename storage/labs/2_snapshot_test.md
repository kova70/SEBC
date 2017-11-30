`hdfs dfs -mkdir precious  
hdfs dfs -ls`
<br>
Found 5 items
drwx------   - rodo-dev supergroup          0 2017-11-28 17:17 .staging
drwxr-xr-x   - rodo-dev supergroup          0 2017-11-28 17:32 precious
drwxr-xr-x   - rodo-dev supergroup          0 2017-11-28 17:06 terasort-input
drwxr-xr-x   - rodo-dev supergroup          0 2017-11-28 17:13 terasort-output
drwxr-xr-x   - rodo-dev supergroup          0 2017-11-28 17:17 terasort-validate

`Adolfo:Curso Cloudera $ scp SEBC-master\ \(5\).zip -u rodo-dev@rodonode1.cloudapp.net:/home/rodo-dev` 
Password: 
SEBC-master (5).zip                                                                                                                                100%  464KB 603.1KB/s   00:

<code>
[rodo-dev@rodonode1 ~]$ hdfs dfs -put SEBC-master.zip 
[rodo-dev@rodonode1 ~]$ hdfs dfs -mv SEBC-master.zip /user/rodo-dev/precious 
[rodo-dev@rodonode1 ~]$ hdfs dfs -ls /user/rodo-dev/precious
Found 1 items
-rw-r--r--   3 rodo-dev supergroup     474833 2017-11-28 17:48 /user/rodo-dev/precious/SEBC-master.zip

[rodo-dev@rodonode1 ~]$ hdfs dfs -rm -skipTrash /user/rodo-dev/precious/SEBC-master.zip
Deleted /user/rodo-dev/precious/SEBC-master.zip
</code>
