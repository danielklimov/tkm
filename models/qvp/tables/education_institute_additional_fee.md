
education_institute_additional_fee
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | uuid | V |  | 
2|`education_institute_id` | uuid |  | [`education_institute`](education_institute.md) | 
3|`education_level_id` | integer |  | [`education_level`](education_level.md) | 
4|`major_id` | integer |  | [`major`](major.md) | 
5|`updated_by_id` | uuid |  | [`users`](users.md) | 
6|`fee` | integer |  |  | 
7|`is_published` | boolean |  |  | 
8|`created_at` | timestamp |  |  | 
9|`updated_at` | timestamp |  |  | 
10|`deleted_at` | timestamp |  |  | 
11|`ministry_id` | varchar |  |  | 
