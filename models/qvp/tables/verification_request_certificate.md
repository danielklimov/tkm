
verification_request_certificate
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | uuid | V |  | 
2|`verification_request_id` | uuid |  | [`verification_request`](verification_request.md) | 
3|`file` | varchar |  |  | 
4|`first_name` | varchar |  |  | 
5|`last_name` | varchar |  |  | 
6|`nationality` | varchar |  |  | 
7|`passport_number` | varchar |  |  | 
8|`major_name` | varchar |  |  | 
9|`created_at` | timestamp |  |  | 
10|`deleted_at` | timestamp |  |  | 
11|`random_id` | integer |  |  | 
12|`country_code` | varchar |  |  | 
13|`should_display_major` | boolean |  |  | 
