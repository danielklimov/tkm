passports
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | Auto-generated or created from source data during migration
2|`first_name` | varchar |  |  | First name of the passport owner
3|`last_name` | varchar |  |  | Last name of the passport owner
4|`passport_number` | varchar |  |  | Document number
5|`country_id` | uuid |  | [`countries`](countries.md) | The country that issued the passport.
6|`issue_date` | date |  |  | Document issue date
7|`expiration_date` | date |  |  | Document expiration date
8|`passport_file_id` | uuid |  | [`file_storage`](file_storage.md) | Passport photo
9|`created_by_user_id` | uuid |  | [`users`](users.md) | The user that created this record. It does not necessarily mean that this user is the owner of the passport.
10|`created_at` | timestamp |  |  | 
11|`updated_at` | timestamp |  |  | 
12|`deleted_status` | varchar |  |  | ACTIVE, DELETED
