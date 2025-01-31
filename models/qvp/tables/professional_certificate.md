
professional_certificate
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | integer | V |  | 
2|`uuid` | uuid |  |  | 
3|`name_english` | varchar |  |  | 
4|`name_arabic` | varchar |  |  | 
5|`institute_name_english` | varchar |  |  | 
6|`institute_name_arabic` | varchar |  |  | 
7|`online_version` | boolean |  |  | 
8|`link` | varchar |  |  | 
9|`published` | boolean |  |  | 
10|`created_at` | timestamp |  |  | 
11|`updated_by_id` | uuid |  | [`users`](users.md) | 
12|`updated_at` | timestamp |  |  | 
13|`deleted_at` | timestamp |  |  | 
