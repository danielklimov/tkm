
education_institute_fee
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | uuid | V |  | 
2|`education_level_id` | integer |  | [`education_level`](education_level.md) | 
3|`major_id` | integer |  | [`major`](major.md) | 
4|`user_id` | uuid |  | [`users`](users.md) | 
5|`name` | varchar |  |  | 
6|`country` | varchar |  |  | 
7|`city` | varchar |  |  | 
8|`place_id` | varchar |  |  | 
9|`fee` | integer |  |  | 
10|`is_published` | boolean |  |  | 
11|`created_at` | timestamp |  |  | 
12|`updated_at` | timestamp |  |  | 
