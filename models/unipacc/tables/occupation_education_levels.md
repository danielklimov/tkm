occupation_education_levels
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | Surrogate key
2|`occupation_id` | uuid |  | [`occupations`](occupations.md) | 
3|`education_level_id` | uuid |  | [`education_levels`](education_levels.md) | 
4|`created_at` | timestamp |  |  | 
5|`updated_at` | timestamp |  |  | 
6|`deleted_status` | varchar |  |  | ACTIVE, DELETED
