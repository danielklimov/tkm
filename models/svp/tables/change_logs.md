
change_logs
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | bigint | V |  | 
2|`loggable_type` | varchar |  |  | 
3|`loggable_id` | bigint |  |  | 
4|`old_values` | jsonb |  |  | 
5|`new_values` | jsonb |  |  | 
6|`created_at` | timestamp |  |  | 
7|`updated_at` | timestamp |  |  | 
8|`user_id` | bigint |  | [`users`](users.md) | 
9|`reason` | varchar |  |  | 
