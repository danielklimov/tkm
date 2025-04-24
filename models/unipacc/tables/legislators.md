legislators
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | bigint | V |  | autogen
2|`user_id` | bigint |  | [`users`](users.md) | The user that created or updated the record
3|`name_en` | varchar |  |  | 
4|`name_ar` | varchar |  |  | 
5|`address` | varchar |  |  | Street address
6|`postal_code` | varchar |  |  | 
7|`is_active` | integer |  |  | TODO: 0, 1 and 2 - what does it mean? Is it active, not active, deleted?
8|`rejection_reason` | text |  |  | Free text
9|`city` | varchar |  |  | 
10|`country_id` | bigint |  | [`countries`](countries.md) | 
11|`show_logo` | boolean |  |  | 
12|`created_at` | timestamp |  |  | 
13|`updated_at` | timestamp |  |  | 
14|`deleted_status` | varchar |  |  | ACTIVE, DELETED
