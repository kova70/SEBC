```
[george@rodonode1 ~]$ beeline 
Beeline version 1.1.0-cdh5.12.1 by Apache Hive
beeline> !connect jdbc:hive2://localhost:10000/default;principal=hive/rodonode1.rodo.com@RODO.COM
scan complete in 2ms
Connecting to jdbc:hive2://localhost:10000/default;principal=hive/rodonode1.rodo.com@RODO.COM
Connected to: Apache Hive (version 1.1.0-cdh5.12.1)
Driver: Hive JDBC (version 1.1.0-cdh5.12.1)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://localhost:10000/default> show tables;
INFO  : Compiling command(queryId=hive_20171130010202_70764877-39ce-486f-a30c-012551a6a2a9): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20171130010202_70764877-39ce-486f-a30c-012551a6a2a9); Time taken: 0.076 seconds
INFO  : Executing command(queryId=hive_20171130010202_70764877-39ce-486f-a30c-012551a6a2a9): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20171130010202_70764877-39ce-486f-a30c-012551a6a2a9); Time taken: 0.125 seconds
INFO  : OK
+------------+--+
|  tab_name  |
+------------+--+
| sample_01  |
| sample_07  |
+------------+--+
2 rows selected (0.225 seconds)

[ferdinand@rodonode1 ~]$ kinit 
Password for ferdinand@RODO.COM: 
[ferdinand@rodonode1 ~]$ beeline
Beeline version 1.1.0-cdh5.12.1 by Apache Hive
beeline> !connect jdbc:hive2://localhost:10000/default;principal=hive/rodonode1.rodo.com@RODO.COM
scan complete in 2ms
Connecting to jdbc:hive2://localhost:10000/default;principal=hive/rodonode1.rodo.com@RODO.COM
Connected to: Apache Hive (version 1.1.0-cdh5.12.1)
Driver: Hive JDBC (version 1.1.0-cdh5.12.1)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://localhost:10000/default> show tables;
INFO  : Compiling command(queryId=hive_20171130005858_94b00e9f-f697-48c2-9dbc-e49291ef2f98): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20171130005858_94b00e9f-f697-48c2-9dbc-e49291ef2f98); Time taken: 0.079 seconds
INFO  : Executing command(queryId=hive_20171130005858_94b00e9f-f697-48c2-9dbc-e49291ef2f98): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20171130005858_94b00e9f-f697-48c2-9dbc-e49291ef2f98); Time taken: 0.148 seconds
INFO  : OK
+------------+--+
|  tab_name  |
+------------+--+
| sample_07  |
+------------+--+
1 row selected (0.337 seconds)
0: jdbc:hive2://localhost:10000/default> 
```

