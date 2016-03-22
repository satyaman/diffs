## <center> <a name="performance"/> Terasort Tests

* Terasort first run
	* <code>time hadoop jar hadoop-examples.jar terasort /user/hduser/terasort-input /user/hduser/terasort-output</code>
	* <div>16/03/22 20:23:53 INFO terasort.TeraSort: starting
			16/03/22 20:23:54 INFO input.FileInputFormat: Total input paths to process : 2
			Spent 175ms computing base-splits.
			Spent 2ms computing TeraScheduler splits.
			Computing input splits took 178ms
			Sampling 8 splits of 8
			Making 6 from 100000 sampled records
			Computing parititions took 754ms
			Spent 935ms computing partitions.
			16/03/22 20:23:55 INFO client.RMProxy: Connecting to ResourceManager at ip-10-0-0-85.ec2.internal/10.0.0.85:8032
			16/03/22 20:23:56 INFO mapreduce.JobSubmitter: number of splits:8
			16/03/22 20:23:56 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1458677897535_0001
			16/03/22 20:23:56 INFO impl.YarnClientImpl: Submitted application application_1458677897535_0001
			16/03/22 20:23:56 INFO mapreduce.Job: The url to track the job: http://ip-10-0-0-85.ec2.internal:8088/proxy/application_1458677897535_0001/
			16/03/22 20:23:56 INFO mapreduce.Job: Running job: job_1458677897535_0001
			16/03/22 20:24:03 INFO mapreduce.Job: Job job_1458677897535_0001 running in uber mode : false
			###Job Progress###
			16/03/22 20:24:35 INFO mapreduce.Job: Job job_1458677897535_0001 completed successfully
			16/03/22 20:24:35 INFO mapreduce.Job: Counters: 49
				File System Counters
					FILE: Number of bytes read=439890465
					FILE: Number of bytes written=878436999
					FILE: Number of read operations=0
					FILE: Number of large read operations=0
					FILE: Number of write operations=0
					HDFS: Number of bytes read=1000001136
					HDFS: Number of bytes written=1000000000
					HDFS: Number of read operations=42
					HDFS: Number of large read operations=0
					HDFS: Number of write operations=12
				Job Counters 
					Launched map tasks=8
					Launched reduce tasks=6
					Data-local map tasks=8
					Total time spent by all maps in occupied slots (ms)=101935
					Total time spent by all reduces in occupied slots (ms)=66185
					Total time spent by all map tasks (ms)=101935
					Total time spent by all reduce tasks (ms)=66185
					Total vcore-seconds taken by all map tasks=101935
					Total vcore-seconds taken by all reduce tasks=66185
					Total megabyte-seconds taken by all map tasks=104381440
					Total megabyte-seconds taken by all reduce tasks=67773440
				Map-Reduce Framework
					Map input records=10000000
					Map output records=10000000
					Map output bytes=1020000000
					Map output materialized bytes=436915218
					Input split bytes=1136
					Combine input records=0
					Combine output records=0
					Reduce input groups=10000000
					Reduce shuffle bytes=436915218
					Reduce input records=10000000
					Reduce output records=10000000
					Spilled Records=20000000
					Shuffled Maps =48
					Failed Shuffles=0
					Merged Map outputs=48
					GC time elapsed (ms)=2775
					CPU time spent (ms)=109250
					Physical memory (bytes) snapshot=7161978880
					Virtual memory (bytes) snapshot=22159327232
					Total committed heap usage (bytes)=7721713664
				Shuffle Errors
					BAD_ID=0
					CONNECTION=0
					IO_ERROR=0
					WRONG_LENGTH=0
					WRONG_MAP=0
					WRONG_REDUCE=0
				File Input Format Counters 
					Bytes Read=1000000000
				File Output Format Counters 
					Bytes Written=1000000000
			16/03/22 20:24:35 INFO terasort.TeraSort: done</div>
		* Time taken 
			* real	0m43.303s
			* user	0m7.821s
			* sys	0m0.311s
* Terasort second run
	* <code>time hadoop jar hadoop-examples.jar terasort /user/hduser/terasort-input /user/hduser/terasort-output</code>
	* <code>16/03/22 20:28:07 INFO terasort.TeraSort: starting
			16/03/22 20:28:08 INFO input.FileInputFormat: Total input paths to process : 2
			Spent 134ms computing base-splits.
			Spent 3ms computing TeraScheduler splits.
			Computing input splits took 138ms
			Sampling 8 splits of 8
			Making 6 from 100000 sampled records
			Computing parititions took 643ms
			Spent 783ms computing partitions.
			16/03/22 20:28:09 INFO client.RMProxy: Connecting to ResourceManager at ip-10-0-0-85.ec2.internal/10.0.0.85:8032
			16/03/22 20:28:10 INFO mapreduce.JobSubmitter: number of splits:8
			16/03/22 20:28:10 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1458677897535_0002
			16/03/22 20:28:10 INFO impl.YarnClientImpl: Submitted application application_1458677897535_0002
			16/03/22 20:28:10 INFO mapreduce.Job: The url to track the job: http://ip-10-0-0-85.ec2.internal:8088/proxy/application_1458677897535_0002/
			16/03/22 20:28:10 INFO mapreduce.Job: Running job: job_1458677897535_0002
			16/03/22 20:28:16 INFO mapreduce.Job: Job job_1458677897535_0002 running in uber mode : false
			###Job Progress###
			16/03/22 20:28:47 INFO mapreduce.Job: Job job_1458677897535_0002 completed successfully
			16/03/22 20:28:47 INFO mapreduce.Job: Counters: 49
				File System Counters
					FILE: Number of bytes read=439890465
					FILE: Number of bytes written=878436999
					FILE: Number of read operations=0
					FILE: Number of large read operations=0
					FILE: Number of write operations=0
					HDFS: Number of bytes read=1000001136
					HDFS: Number of bytes written=1000000000
					HDFS: Number of read operations=42
					HDFS: Number of large read operations=0
					HDFS: Number of write operations=12
				Job Counters 
					Launched map tasks=8
					Launched reduce tasks=6
					Data-local map tasks=8
					Total time spent by all maps in occupied slots (ms)=97642
					Total time spent by all reduces in occupied slots (ms)=63550
					Total time spent by all map tasks (ms)=97642
					Total time spent by all reduce tasks (ms)=63550
					Total vcore-seconds taken by all map tasks=97642
					Total vcore-seconds taken by all reduce tasks=63550
					Total megabyte-seconds taken by all map tasks=99985408
					Total megabyte-seconds taken by all reduce tasks=65075200
				Map-Reduce Framework
					Map input records=10000000
					Map output records=10000000
					Map output bytes=1020000000
					Map output materialized bytes=436915218
					Input split bytes=1136
					Combine input records=0
					Combine output records=0
					Reduce input groups=10000000
					Reduce shuffle bytes=436915218
					Reduce input records=10000000
					Reduce output records=10000000
					Spilled Records=20000000
					Shuffled Maps =48
					Failed Shuffles=0
					Merged Map outputs=48
					GC time elapsed (ms)=2597
					CPU time spent (ms)=107570
					Physical memory (bytes) snapshot=6981435392
					Virtual memory (bytes) snapshot=22154817536
					Total committed heap usage (bytes)=7598505984
				Shuffle Errors
					BAD_ID=0
					CONNECTION=0
					IO_ERROR=0
					WRONG_LENGTH=0
					WRONG_MAP=0
					WRONG_REDUCE=0
				File Input Format Counters 
					Bytes Read=1000000000
				File Output Format Counters 
					Bytes Written=1000000000
			16/03/22 20:28:47 INFO terasort.TeraSort: done</code>
	* Time taken
		* real	0m41.357s
		* user	0m7.674s
		* sys	0m0.311s
* Terasort third run - AFTER Short Circuit Reads is ENABLED
	* <code>time hadoop jar hadoop-examples.jar terasort /user/hduser/terasort-input /user/hduser/terasort-output</code>
	* <code>16/03/22 20:36:07 INFO terasort.TeraSort: starting
			16/03/22 20:36:08 INFO input.FileInputFormat: Total input paths to process : 2
			Spent 124ms computing base-splits.
			Spent 2ms computing TeraScheduler splits.
			Computing input splits took 127ms
			Sampling 8 splits of 8
			Making 6 from 100000 sampled records
			Computing parititions took 792ms
			Spent 921ms computing partitions.
			16/03/22 20:36:09 INFO client.RMProxy: Connecting to ResourceManager at ip-10-0-0-85.ec2.internal/10.0.0.85:8032
			16/03/22 20:36:10 INFO mapreduce.JobSubmitter: number of splits:8
			16/03/22 20:36:10 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1458678756208_0002
			16/03/22 20:36:10 INFO impl.YarnClientImpl: Submitted application application_1458678756208_0002
			16/03/22 20:36:10 INFO mapreduce.Job: The url to track the job: http://ip-10-0-0-85.ec2.internal:8088/proxy/application_1458678756208_0002/
			16/03/22 20:36:10 INFO mapreduce.Job: Running job: job_1458678756208_0002
			16/03/22 20:36:17 INFO mapreduce.Job: Job job_1458678756208_0002 running in uber mode : false
			16/03/22 20:36:17 INFO mapreduce.Job:  map 0% reduce 0%
			16/03/22 20:36:29 INFO mapreduce.Job:  map 25% reduce 0%
			16/03/22 20:36:31 INFO mapreduce.Job:  map 75% reduce 0%
			16/03/22 20:36:32 INFO mapreduce.Job:  map 92% reduce 0%
			16/03/22 20:36:33 INFO mapreduce.Job:  map 100% reduce 0%
			16/03/22 20:36:45 INFO mapreduce.Job:  map 100% reduce 83%
			16/03/22 20:36:46 INFO mapreduce.Job:  map 100% reduce 100%
			16/03/22 20:36:46 INFO mapreduce.Job: Job job_1458678756208_0002 completed successfully
			16/03/22 20:36:46 INFO mapreduce.Job: Counters: 49
				File System Counters
					FILE: Number of bytes read=439890465
					FILE: Number of bytes written=878439015
					FILE: Number of read operations=0
					FILE: Number of large read operations=0
					FILE: Number of write operations=0
					HDFS: Number of bytes read=1000001136
					HDFS: Number of bytes written=1000000000
					HDFS: Number of read operations=42
					HDFS: Number of large read operations=0
					HDFS: Number of write operations=12
				Job Counters 
					Launched map tasks=8
					Launched reduce tasks=6
					Data-local map tasks=8
					Total time spent by all maps in occupied slots (ms)=96629
					Total time spent by all reduces in occupied slots (ms)=63333
					Total time spent by all map tasks (ms)=96629
					Total time spent by all reduce tasks (ms)=63333
					Total vcore-seconds taken by all map tasks=96629
					Total vcore-seconds taken by all reduce tasks=63333
					Total megabyte-seconds taken by all map tasks=98948096
					Total megabyte-seconds taken by all reduce tasks=64852992
				Map-Reduce Framework
					Map input records=10000000
					Map output records=10000000
					Map output bytes=1020000000
					Map output materialized bytes=436915218
					Input split bytes=1136
					Combine input records=0
					Combine output records=0
					Reduce input groups=10000000
					Reduce shuffle bytes=436915218
					Reduce input records=10000000
					Reduce output records=10000000
					Spilled Records=20000000
					Shuffled Maps =48
					Failed Shuffles=0
					Merged Map outputs=48
					GC time elapsed (ms)=3074
					CPU time spent (ms)=107210
					Physical memory (bytes) snapshot=7295590400
					Virtual memory (bytes) snapshot=22189187072
					Total committed heap usage (bytes)=7578583040
				Shuffle Errors
					BAD_ID=0
					CONNECTION=0
					IO_ERROR=0
					WRONG_LENGTH=0
					WRONG_MAP=0
					WRONG_REDUCE=0
				File Input Format Counters 
					Bytes Read=1000000000
				File Output Format Counters 
					Bytes Written=1000000000
			16/03/22 20:36:46 INFO terasort.TeraSort: done</code>
	* Time taken
		* real	0m40.291s
		* user	0m7.587s
		* sys	0m0.275s