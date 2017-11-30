`hadoop jar hadoop-examples.jar teragen 100000000 /user/rodo-dev/terasort-input`<br>
17/11/28 17:05:00 INFO client.RMProxy: Connecting to ResourceManager at rodonode1.RodoNode1.d3.internal.cloudapp.net/10.2.0.4:8032
17/11/28 17:05:00 INFO terasort.TeraGen: Generating 100000000 using 2
17/11/28 17:05:01 INFO mapreduce.JobSubmitter: number of splits:2
17/11/28 17:05:01 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1511882332135_0004
17/11/28 17:05:01 INFO impl.YarnClientImpl: Submitted application application_1511882332135_0004
17/11/28 17:05:01 INFO mapreduce.Job: The url to track the job: http://rodonode1.RodoNode1.d3.internal.cloudapp.net:8088/proxy/application_1511882332135_0004/
17/11/28 17:05:01 INFO mapreduce.Job: Running job: job_1511882332135_0004
17/11/28 17:05:06 INFO mapreduce.Job: Job job_1511882332135_0004 running in uber mode : false
17/11/28 17:05:06 INFO mapreduce.Job:  map 0% reduce 0%
17/11/28 17:05:23 INFO mapreduce.Job:  map 20% reduce 0%
17/11/28 17:05:29 INFO mapreduce.Job:  map 30% reduce 0%
17/11/28 17:05:35 INFO mapreduce.Job:  map 41% reduce 0%
17/11/28 17:05:42 INFO mapreduce.Job:  map 48% reduce 0%
17/11/28 17:05:48 INFO mapreduce.Job:  map 58% reduce 0%
17/11/28 17:05:54 INFO mapreduce.Job:  map 66% reduce 0%
17/11/28 17:06:00 INFO mapreduce.Job:  map 74% reduce 0%
17/11/28 17:06:06 INFO mapreduce.Job:  map 83% reduce 0%
17/11/28 17:06:12 INFO mapreduce.Job:  map 89% reduce 0%
17/11/28 17:06:18 INFO mapreduce.Job:  map 97% reduce 0%
17/11/28 17:06:22 INFO mapreduce.Job:  map 100% reduce 0%
17/11/28 17:06:23 INFO mapreduce.Job: Job job_1511882332135_0004 completed successfully
17/11/28 17:06:23 INFO mapreduce.Job: Counters: 31
	File System Counters
		FILE: Number of bytes read=0
		FILE: Number of bytes written=291286
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=170
		HDFS: Number of bytes written=10000000000
		HDFS: Number of read operations=8
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=4
	Job Counters 
		Launched map tasks=2
		Other local map tasks=2
		Total time spent by all maps in occupied slots (ms)=141859
		Total time spent by all reduces in occupied slots (ms)=0
		Total time spent by all map tasks (ms)=141859
		Total vcore-milliseconds taken by all map tasks=141859
		Total megabyte-milliseconds taken by all map tasks=145263616
	Map-Reduce Framework
		Map input records=100000000
		Map output records=100000000
		Input split bytes=170
		Spilled Records=0
		Failed Shuffles=0
		Merged Map outputs=0
		GC time elapsed (ms)=943
		CPU time spent (ms)=135340
		Physical memory (bytes) snapshot=465395712
		Virtual memory (bytes) snapshot=3186896896
		Total committed heap usage (bytes)=878706688
	org.apache.hadoop.examples.terasort.TeraGen$Counters
		CHECKSUM=214760662691937609
	File Input Format Counters 
		Bytes Read=0
	File Output Format Counters 
		Bytes Written=10000000000<br>
    
`hadoop jar hadoop-examples.jar terasort /user/rodo-dev/terasort-input /user/rodo-dev/terasort-output`<br>
17/11/28 17:11:44 INFO terasort.TeraSort: starting
17/11/28 17:11:46 INFO input.FileInputFormat: Total input paths to process : 2
Spent 197ms computing base-splits.
Spent 2ms computing TeraScheduler splits.
Computing input splits took 200ms
Sampling 10 splits of 76
Making 12 from 100000 sampled records
Computing parititions took 676ms
Spent 879ms computing partitions.
17/11/28 17:11:46 INFO client.RMProxy: Connecting to ResourceManager at rodonode1.RodoNode1.d3.internal.cloudapp.net/10.2.0.4:8032
17/11/28 17:11:47 INFO mapreduce.JobSubmitter: number of splits:76
17/11/28 17:11:47 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1511882332135_0005
17/11/28 17:11:47 INFO impl.YarnClientImpl: Submitted application application_1511882332135_0005
17/11/28 17:11:47 INFO mapreduce.Job: The url to track the job: http://rodonode1.RodoNode1.d3.internal.cloudapp.net:8088/proxy/application_1511882332135_0005/
17/11/28 17:11:47 INFO mapreduce.Job: Running job: job_1511882332135_0005
17/11/28 17:11:52 INFO mapreduce.Job: Job job_1511882332135_0005 running in uber mode : false
17/11/28 17:11:52 INFO mapreduce.Job:  map 0% reduce 0%
17/11/28 17:12:09 INFO mapreduce.Job:  map 11% reduce 0%
17/11/28 17:12:10 INFO mapreduce.Job:  map 18% reduce 0%
17/11/28 17:12:11 INFO mapreduce.Job:  map 20% reduce 0%
17/11/28 17:12:12 INFO mapreduce.Job:  map 26% reduce 0%
17/11/28 17:12:14 INFO mapreduce.Job:  map 30% reduce 0%
17/11/28 17:12:23 INFO mapreduce.Job:  map 36% reduce 0%
17/11/28 17:12:24 INFO mapreduce.Job:  map 37% reduce 0%
17/11/28 17:12:25 INFO mapreduce.Job:  map 49% reduce 0%
17/11/28 17:12:27 INFO mapreduce.Job:  map 50% reduce 0%
17/11/28 17:12:29 INFO mapreduce.Job:  map 51% reduce 0%
17/11/28 17:12:30 INFO mapreduce.Job:  map 58% reduce 0%
17/11/28 17:12:31 INFO mapreduce.Job:  map 61% reduce 0%
17/11/28 17:12:38 INFO mapreduce.Job:  map 66% reduce 0%
17/11/28 17:12:39 INFO mapreduce.Job:  map 72% reduce 0%
17/11/28 17:12:40 INFO mapreduce.Job:  map 79% reduce 0%
17/11/28 17:12:41 INFO mapreduce.Job:  map 80% reduce 0%
17/11/28 17:12:46 INFO mapreduce.Job:  map 82% reduce 0%
17/11/28 17:12:48 INFO mapreduce.Job:  map 89% reduce 0%
17/11/28 17:12:49 INFO mapreduce.Job:  map 92% reduce 0%
17/11/28 17:12:50 INFO mapreduce.Job:  map 93% reduce 0%
17/11/28 17:12:54 INFO mapreduce.Job:  map 97% reduce 0%
17/11/28 17:12:55 INFO mapreduce.Job:  map 100% reduce 0%
17/11/28 17:13:01 INFO mapreduce.Job:  map 100% reduce 5%
17/11/28 17:13:02 INFO mapreduce.Job:  map 100% reduce 31%
17/11/28 17:13:03 INFO mapreduce.Job:  map 100% reduce 42%
17/11/28 17:13:04 INFO mapreduce.Job:  map 100% reduce 54%
17/11/28 17:13:07 INFO mapreduce.Job:  map 100% reduce 67%
17/11/28 17:13:08 INFO mapreduce.Job:  map 100% reduce 75%
17/11/28 17:13:09 INFO mapreduce.Job:  map 100% reduce 79%
17/11/28 17:13:10 INFO mapreduce.Job:  map 100% reduce 81%
17/11/28 17:13:13 INFO mapreduce.Job:  map 100% reduce 86%
17/11/28 17:13:14 INFO mapreduce.Job:  map 100% reduce 93%
17/11/28 17:13:15 INFO mapreduce.Job:  map 100% reduce 95%
17/11/28 17:13:17 INFO mapreduce.Job:  map 100% reduce 97%
17/11/28 17:13:18 INFO mapreduce.Job:  map 100% reduce 98%
17/11/28 17:13:19 INFO mapreduce.Job:  map 100% reduce 99%
17/11/28 17:13:20 INFO mapreduce.Job:  map 100% reduce 100%
17/11/28 17:13:33 INFO mapreduce.Job: Job job_1511882332135_0005 completed successfully
17/11/28 17:13:33 INFO mapreduce.Job: Counters: 49
	File System Counters
		FILE: Number of bytes read=4445440500
		FILE: Number of bytes written=8829270207
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=10000012388
		HDFS: Number of bytes written=10000000000
		HDFS: Number of read operations=264
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=24
	Job Counters 
		Launched map tasks=76
		Launched reduce tasks=12
		Data-local map tasks=76
		Total time spent by all maps in occupied slots (ms)=1095298
		Total time spent by all reduces in occupied slots (ms)=416691
		Total time spent by all map tasks (ms)=1095298
		Total time spent by all reduce tasks (ms)=416691
		Total vcore-milliseconds taken by all map tasks=1095298
		Total vcore-milliseconds taken by all reduce tasks=416691
		Total megabyte-milliseconds taken by all map tasks=1121585152
		Total megabyte-milliseconds taken by all reduce tasks=426691584
	Map-Reduce Framework
		Map input records=100000000
		Map output records=100000000
		Map output bytes=10200000000
		Map output materialized bytes=4370860826
		Input split bytes=12388
		Combine input records=0
		Combine output records=0
		Reduce input groups=100000000
		Reduce shuffle bytes=4370860826
		Reduce input records=100000000
		Reduce output records=100000000
		Spilled Records=200000000
		Shuffled Maps =912
		Failed Shuffles=0
		Merged Map outputs=912
		GC time elapsed (ms)=25043
		CPU time spent (ms)=966300
		Physical memory (bytes) snapshot=57995743232
		Virtual memory (bytes) snapshot=140766261248
		Total committed heap usage (bytes)=56601608192
	Shuffle Errors
		BAD_ID=0
		CONNECTION=0
		IO_ERROR=0
		WRONG_LENGTH=0
		WRONG_MAP=0
		WRONG_REDUCE=0
	File Input Format Counters 
		Bytes Read=10000000000
	File Output Format Counters 
		Bytes Written=10000000000
17/11/28 17:13:33 INFO terasort.TeraSort: done

`hadoop jar hadoop-examples.jar teravalidate /user/rodo-dev/terasort-output /user/rodo-dev/terasort-validate`<br>
17/11/28 17:16:44 INFO client.RMProxy: Connecting to ResourceManager at rodonode1.RodoNode1.d3.internal.cloudapp.net/10.2.0.4:8032
17/11/28 17:16:44 INFO input.FileInputFormat: Total input paths to process : 12
Spent 37ms computing base-splits.
Spent 2ms computing TeraScheduler splits.
17/11/28 17:16:45 INFO mapreduce.JobSubmitter: number of splits:12
17/11/28 17:16:45 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1511882332135_0006
17/11/28 17:16:45 INFO impl.YarnClientImpl: Submitted application application_1511882332135_0006
17/11/28 17:16:45 INFO mapreduce.Job: The url to track the job: http://rodonode1.RodoNode1.d3.internal.cloudapp.net:8088/proxy/application_1511882332135_0006/
17/11/28 17:16:45 INFO mapreduce.Job: Running job: job_1511882332135_0006
17/11/28 17:16:50 INFO mapreduce.Job: Job job_1511882332135_0006 running in uber mode : false
17/11/28 17:16:50 INFO mapreduce.Job:  map 0% reduce 0%
17/11/28 17:17:02 INFO mapreduce.Job:  map 8% reduce 0%
17/11/28 17:17:03 INFO mapreduce.Job:  map 25% reduce 0%
17/11/28 17:17:04 INFO mapreduce.Job:  map 58% reduce 0%
17/11/28 17:17:05 INFO mapreduce.Job:  map 67% reduce 0%
17/11/28 17:17:06 INFO mapreduce.Job:  map 92% reduce 0%
17/11/28 17:17:07 INFO mapreduce.Job:  map 100% reduce 0%
17/11/28 17:17:11 INFO mapreduce.Job:  map 100% reduce 100%
17/11/28 17:17:12 INFO mapreduce.Job: Job job_1511882332135_0006 completed successfully
17/11/28 17:17:13 INFO mapreduce.Job: Counters: 50
	File System Counters
		FILE: Number of bytes read=678
		FILE: Number of bytes written=1901431
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=10000001968
		HDFS: Number of bytes written=25
		HDFS: Number of read operations=39
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=2
	Job Counters 
		Launched map tasks=12
		Launched reduce tasks=1
		Data-local map tasks=8
		Rack-local map tasks=4
		Total time spent by all maps in occupied slots (ms)=144839
		Total time spent by all reduces in occupied slots (ms)=2479
		Total time spent by all map tasks (ms)=144839
		Total time spent by all reduce tasks (ms)=2479
		Total vcore-milliseconds taken by all map tasks=144839
		Total vcore-milliseconds taken by all reduce tasks=2479
		Total megabyte-milliseconds taken by all map tasks=148315136
		Total megabyte-milliseconds taken by all reduce tasks=2538496
	Map-Reduce Framework
		Map input records=100000000
		Map output records=36
		Map output bytes=984
		Map output materialized bytes=1152
		Input split bytes=1968
		Combine input records=0
		Combine output records=0
		Reduce input groups=25
		Reduce shuffle bytes=1152
		Reduce input records=36
		Reduce output records=1
		Spilled Records=72
		Shuffled Maps =12
		Failed Shuffles=0
		Merged Map outputs=12
		GC time elapsed (ms)=2219
		CPU time spent (ms)=110650
		Physical memory (bytes) snapshot=7913304064
		Virtual memory (bytes) snapshot=20790960128
		Total committed heap usage (bytes)=7949254656
	Shuffle Errors
		BAD_ID=0
		CONNECTION=0
		IO_ERROR=0
		WRONG_LENGTH=0
		WRONG_MAP=0
		WRONG_REDUCE=0
	File Input Format Counters 
		Bytes Read=10000000000
	File Output Format Counters 
		Bytes Written=25
    
`hdfs dfs -ls -h`<br>
Found 4 items
drwx------   - rodo-dev supergroup          0 2017-11-28 17:17 .staging
drwxr-xr-x   - rodo-dev supergroup          0 2017-11-28 17:06 terasort-input
drwxr-xr-x   - rodo-dev supergroup          0 2017-11-28 17:13 terasort-output
drwxr-xr-x   - rodo-dev supergroup          0 2017-11-28 17:17 terasort-validate

`hdfs dfs -ls -h terasort-input`<br>
Found 3 items
-rw-r--r--   3 rodo-dev supergroup          0 2017-11-28 17:06 terasort-input/_SUCCESS
-rw-r--r--   3 rodo-dev supergroup      4.7 G 2017-11-28 17:06 terasort-input/part-m-00000
-rw-r--r--   3 rodo-dev supergroup      4.7 G 2017-11-28 17:06 terasort-input/part-m-00001

    
