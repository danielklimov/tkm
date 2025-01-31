
exam_sessions
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | bigint | V |  | 
2|`end_at` | timestamp |  |  | 
3|`location_link` | varchar |  |  | 
4|`seats` | integer |  |  | 
7|`start_at` | timestamp |  |  | 
8|`test_center_id` | bigint |  | [`test_centers`](test_centers.md) | 
9|`verification_code` | varchar |  |  | 
10|`category_id` | bigint |  | [`categories`](categories.md) | 
11|`created_at` | timestamp |  |  | 
12|`updated_at` | timestamp |  |  | 
13|`status` | integer |  |  | 
14|`repeat` | integer |  |  | 
15|`cancellation_reason` | varchar |  |  | 
17|`reminder_sent` | boolean |  |  | 
18|`cancelled_by_user_id` | bigint |  | [`users`](users.md) | 
19|`repeat_rule_description` | varchar |  |  | 
20|`time_zone_name` | varchar |  |  | 
21|`phase_status` | integer |  |  | 
