
major
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | integer | V |  | 
2|`name_arabic` | varchar |  |  | 
3|`name_english` | varchar |  |  | 
4|`published` | boolean |  |  | 
6|`created_at` | timestamp |  |  | 
7|`updated_at` | timestamp |  |  | 
8|`deleted_at` | timestamp |  |  | 
9|`user_id` | uuid |  |  | 
11|`updated_by_id` | uuid |  | [`users`](users.md) | 
12|`rare_in_saudi_arabia` | boolean |  |  | 
13|`active` | boolean |  |  | 
14|`ministry_id` | varchar |  |  | 
