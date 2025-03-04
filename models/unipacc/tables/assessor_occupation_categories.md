assessor_occupation_categories
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`assessor_id` | uuid | V | [`assessors`](assessors.md) | 
2|`occupation_category_id` | uuid | V | [`occupation_categories`](occupation_categories.md) | 
3|`created_at` | timestamp |  |  | 
4|`updated_at` | timestamp |  |  | 
5|`deleted_status` | integer | V |  | 0 - active record, 1 - deleted record.
