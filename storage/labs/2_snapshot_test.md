# HDFS Lab: Test HDFS Snapshots

- Create a precious directory in HDFS; copy the ZIP course file into it. <br>
  `hdfs dfs -mkdir precious` <br>
  `hdfs dfs -ls` <br>
  Found 5 items 
  drwx------   - rodo-dev supergroup          0 2017-11-28 17:17 .staging <br>
  drwxr-xr-x   - rodo-dev supergroup          0 2017-11-28 17:32 precious <br>
  drwxr-xr-x   - rodo-dev supergroup          0 2017-11-28 17:06 terasort-input <br>
  drwxr-xr-x   - rodo-dev supergroup          0 2017-11-28 17:13 terasort-output <br>
  drwxr-xr-x   - rodo-dev supergroup          0 2017-11-28 17:17 terasort-validate <br>
<br>

- Copy the ZIP course file into it. <br>
Adolfo:Curso Cloudera $ scp SEBC-master\ \(5\).zip -u rodo-dev@rodonode1.cloudapp.net:/home/rodo-dev
Password:<br>
SEBC-master (5).zip<br>                                                                                                                             100%  464KB 603.1KB/s   00:<br>
[rodo-dev@rodonode1 ~]$ hdfs dfs -put SEBC-master.zip <br>
[rodo-dev@rodonode1 ~]$ hdfs dfs -mv SEBC-master.zip /user/rodo-dev/precious <br>
[rodo-dev@rodonode1 ~]$ hdfs dfs -ls /user/rodo-dev/precious <br>
Found 1 items <br>
-rw-r--r--   3 rodo-dev supergroup     474833 2017-11-28 17:48 /user/rodo-dev/precious/SEBC-master.zip 
<br>

- Delete the file <br>
[rodo-dev@rodonode1 ~]$ hdfs dfs -rm -skipTrash /user/rodo-dev/precious/SEBC-master.zip
Deleted /user/rodo-dev/precious/SEBC-master.zip
