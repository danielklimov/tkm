
groups
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | bigint | V |  | 
2|`file_name` | varchar |  |  | 
3|`created_at` | timestamp |  |  | 
4|`updated_at` | timestamp |  |  | 
5|`total_labors` | integer |  |  | 
6|`passed_labors` | integer |  |  | 
7|`payment_status` | integer |  |  | 
8|`legislator_id` | bigint |  | [`legislators`](legislators.md) | 
9|`group_type` | integer |  |  | 
10|`user_id` | bigint |  | [`users`](users.md) | 
