
pg_stat_statements
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`userid` | oid |  |  | 
2|`dbid` | oid |  |  | 
3|`queryid` | bigint |  |  | 
4|`query` | text |  |  | 
5|`plans` | bigint |  |  | 
6|`total_plan_time` | double precision |  |  | 
7|`min_plan_time` | double precision |  |  | 
8|`max_plan_time` | double precision |  |  | 
9|`mean_plan_time` | double precision |  |  | 
10|`stddev_plan_time` | double precision |  |  | 
11|`calls` | bigint |  |  | 
12|`total_exec_time` | double precision |  |  | 
13|`min_exec_time` | double precision |  |  | 
14|`max_exec_time` | double precision |  |  | 
15|`mean_exec_time` | double precision |  |  | 
16|`stddev_exec_time` | double precision |  |  | 
17|`rows` | bigint |  |  | 
18|`shared_blks_hit` | bigint |  |  | 
19|`shared_blks_read` | bigint |  |  | 
20|`shared_blks_dirtied` | bigint |  |  | 
21|`shared_blks_written` | bigint |  |  | 
22|`local_blks_hit` | bigint |  |  | 
23|`local_blks_read` | bigint |  |  | 
24|`local_blks_dirtied` | bigint |  |  | 
25|`local_blks_written` | bigint |  |  | 
26|`temp_blks_read` | bigint |  |  | 
27|`temp_blks_written` | bigint |  |  | 
28|`blk_read_time` | double precision |  |  | 
29|`blk_write_time` | double precision |  |  | 
30|`wal_records` | bigint |  |  | 
31|`wal_fpi` | bigint |  |  | 
32|`wal_bytes` | numeric |  |  | 
