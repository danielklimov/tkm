
legislators
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | bigint | V |  | 
2|`user_id` | bigint |  | [`users`](users.md) | 
3|`english_name` | varchar |  |  | 
4|`arabic_name` | varchar |  |  | 
5|`address` | varchar |  |  | 
6|`postal_code` | varchar |  |  | 
7|`status` | integer |  |  | 
8|`rejection_reason` | text |  |  | 
9|`city` | varchar |  |  | 
10|`created_at` | timestamp |  |  | 
11|`updated_at` | timestamp |  |  | 
12|`country_id` | bigint |  | [`countries`](countries.md) | 
13|`show_logo` | boolean |  |  | 
