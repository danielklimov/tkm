assessors
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION  | COMMENTS          
---|------|-----------|----|----|--------------|----------
1|`id` | uuid | V |  | Auto-generated or manually generated during migration | 
2|`location_country_id` | uuid |  | [`countries`](countries.md) |  | 
3|`citizenship_country_id` | uuid |  | [`countries`](countries.md) | TODO: does it make sense to keep this field when there is passport_id field? Maybe it does  if, for example, the assessor hasn't entered information about his passport yet. | 
4|`user_id` | uuid |  | [`users`](users.md) | User account used by this assessor to log in. | 
5|`passport_id` | uuid |  | [`passports`](passports.md) | Currently active passport | 
6|`created_at` | timestamp |  |  |  | 
7|`updated_at` | timestamp |  |  |  | 
8|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record. | 
