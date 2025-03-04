passports
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION  | COMMENTS          
---|------|-----------|----|----|--------------|----------
1|`id` | uuid | V |  | Auto-generated or created from source data during migration
2|`first_name` | varchar |  |  | First name of the passport owner
3|`last_name` | varchar |  |  | Last name of the passport owner
4|`passport_number` | varchar |  |  | Document number
5|`country_id` | uuid |  | [`countries`](countries.md) | The country that issued the passport.
6|`issue_date` | date |  |  | Document issue date
7|`expiration_date` | date |  |  | Document expiration date
8|`created_by_user_id` | uuid |  | [`users`](users.md) | The user that created this record. It does not necessarily mean that this user is the owner of the passport.
9|`created_at` | timestamp |  |  | 
10|`updated_at` | timestamp |  |  | 
11|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record.
