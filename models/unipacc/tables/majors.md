majors
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION  | COMMENTS          
---|------|-----------|----|----|--------------|----------
1|`id` | uuid | V |  | manually generated on migration from integer value
2|`name_en` | varchar |  |  | Name in English
3|`name_ar` | varchar |  |  | Name in Arabic
4|`rare_in_sa` | boolean |  |  | Rare in Saudi Arabia
5|`is_published` | boolean |  |  | Shown is web app
6|`updated_by_user_id` | uuid |  | [`users`](users.md) | The user who updated the record last time
7|`created_at` | timestamp |  |  | 
8|`updated_at` | timestamp |  |  | 
9|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record.
