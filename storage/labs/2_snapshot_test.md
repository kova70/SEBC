# HDFS Lab: Test HDFS Snapshots

- Create a precious directory in HDFS; copy the ZIP course file into it.
<code>
  hdfs dfs -mkdir precious <br>
  hdfs dfs -ls` <br>
<br>
Found 5 items
drwx------   - rodo-dev supergroup          0 2017-11-28 17:17 .staging
drwxr-xr-x   - rodo-dev supergroup          0 2017-11-28 17:32 precious
drwxr-xr-x   - rodo-dev supergroup          0 2017-11-28 17:06 terasort-input
drwxr-xr-x   - rodo-dev supergroup          0 2017-11-28 17:13 terasort-output
drwxr-xr-x   - rodo-dev supergroup          0 2017-11-28 17:17 terasort-validate
</code>

- Copy the ZIP course file into it.
<code>
Adolfo:Curso Cloudera $ scp SEBC-master\ \(5\).zip -u rodo-dev@rodonode1.cloudapp.net:/home/rodo-dev`
Password: 
SEBC-master (5).zip                                                                                                                                100%  464KB 603.1KB/s   00:
[rodo-dev@rodonode1 ~]$ hdfs dfs -put SEBC-master.zip 
[rodo-dev@rodonode1 ~]$ hdfs dfs -mv SEBC-master.zip /user/rodo-dev/precious 
[rodo-dev@rodonode1 ~]$ hdfs dfs -ls /user/rodo-dev/precious
Found 1 items
-rw-r--r--   3 rodo-dev supergroup     474833 2017-11-28 17:48 /user/rodo-dev/precious/SEBC-master.zip
</code>
<code>
- Delete the file 
[rodo-dev@rodonode1 ~]$ hdfs dfs -rm -skipTrash /user/rodo-dev/precious/SEBC-master.zip
Deleted /user/rodo-dev/precious/SEBC-master.zip
</code>
