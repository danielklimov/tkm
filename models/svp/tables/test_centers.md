
test_centers
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | bigint | V |  | 
2|`name` | varchar |  |  | 
3|`city` | varchar |  |  | 
4|`address` | varchar |  |  | 
5|`status` | integer |  |  | 
6|`created_at` | timestamp |  |  | 
7|`updated_at` | timestamp |  |  | 
8|`phone_number` | varchar |  |  | 
9|`country_code` | varchar |  |  | 
10|`postal_code` | varchar |  |  | 
11|`user_id` | bigint |  | [`users`](users.md) | 
12|`country_id` | bigint |  | [`countries`](countries.md) | 
13|`legislator_id` | bigint |  | [`legislators`](legislators.md) | 
14|`exam_sessions_count` | integer |  |  | 
