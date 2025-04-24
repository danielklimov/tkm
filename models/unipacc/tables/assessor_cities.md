assessor_cities
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | surrogate key
2|`assessor_id` | uuid |  | [`assessors`](assessors.md) | 
3|`city_name` | varchar |  |  | Name of a city that this assessor is servicing
4|`created_at` | timestamp |  |  | 
5|`updated_at` | timestamp |  |  | 
6|`deleted_status` | varchar |  |  | ACTIVE, DELETED
