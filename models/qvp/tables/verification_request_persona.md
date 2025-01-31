
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
15|`country` | varchar |  |  | 
18|`deleted_at` | timestamp |  |  | 
19|`passport_id` | uuid |  | [`passport`](passport.md) | 
20|`current_location` | varchar |  |  | 
21|`state` | varchar |  |  | 
22|`current_location_validated` | varchar |  |  | 
23|`ip_address` | varchar |  |  | 
24|`request_reason` | varchar |  |  | 
