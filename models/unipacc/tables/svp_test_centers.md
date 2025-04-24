svp_test_centers
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | autoincr
2|`name` | varchar |  |  | Test center name
3|`city` | varchar |  |  | 
4|`address` | varchar |  |  | Street address
5|`is_active` | varchar |  |  | One of: active, inactive, deleted
6|`phone_number` | varchar |  |  | 
7|`postal_code` | varchar |  |  | 
8|`user_id` | uuid |  | [`users`](users.md) | 
9|`country_id` | uuid |  | [`countries`](countries.md) | 
10|`legislator_id` | uuid |  | [`legislators`](legislators.md) | 
11|`latitude` | double |  |  | Test center location - latitude
12|`longitude` | double |  |  | Test center location - longitude
13|`created_at` | timestamp |  |  | 
14|`updated_at` | timestamp |  |  | 
15|`deleted_status` | varchar |  |  | ACTIVE, DELETED
27|`created_at` | timestamp |  |  | 
28|`updated_at` | timestamp |  |  | 
29|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record.
