```
beeline> !connect jdbc:hive2://localhost:10000/default;principal=hive/rodonode1.rodo.com@RODO.COM
Connecting to jdbc:hive2://localhost:10000/default;principal=hive/rodonode1.rodo.com@RODO.COM
Connected to: Apache Hive (version 1.1.0-cdh5.12.1)
Driver: Hive JDBC (version 1.1.0-cdh5.12.1)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://localhost:10000/default> SHOW TABLES
. . . . . . . . . . . . . . . . . . . .> ;
INFO  : Compiling command(queryId=hive_20171130002727_c8aa3525-5d0e-4fdd-abcc-c55ba0dd9d29): SHOW TABLES
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20171130002727_c8aa3525-5d0e-4fdd-abcc-c55ba0dd9d29); Time taken: 0.757 seconds
INFO  : Executing command(queryId=hive_20171130002727_c8aa3525-5d0e-4fdd-abcc-c55ba0dd9d29): SHOW TABLES
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20171130002727_c8aa3525-5d0e-4fdd-abcc-c55ba0dd9d29); Time taken: 0.316 seconds
INFO  : OK
+-----------+--+
| tab_name  |
+-----------+--+
+-----------+--+
No rows selected (2.513 seconds)
0: jdbc:hive2://localhost:10000/default> 
```
