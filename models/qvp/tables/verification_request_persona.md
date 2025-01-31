
verification_request_persona
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | uuid | V |  | 
2|`first_name` | varchar |  |  | 
3|`last_name` | varchar |  |  | 
4|`second_name` | varchar |  |  | 
5|`gender` | varchar |  |  | 
6|`alternate_name` | varchar |  |  | 
7|`maiden_name` | varchar |  |  | 
8|`former_married_name` | varchar |  |  | 
9|`suffix` | varchar |  |  | 
10|`mothers_name` | varchar |  |  | 
11|`date_of_birth` | timestamp |  |  | 
12|`phone_number` | varchar |  |  | 
13|`country_code` | varchar |  |  | 
14|`country` | varchar |  |  | 
15|`deleted_at` | timestamp |  |  | 
16|`passport_id` | uuid |  | [`passport`](passport.md) | 
17|`current_location` | varchar |  |  | 
18|`state` | varchar |  |  | 
19|`current_location_validated` | varchar |  |  | 
20|`ip_address` | varchar |  |  | 
21|`request_reason` | varchar |  |  | 
