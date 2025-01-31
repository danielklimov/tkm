
users
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | uuid | V |  | 
2|`email` | varchar |  |  | 
3|`roles` | text |  |  | 
4|`first_name` | varchar |  |  | 
5|`last_name` | varchar |  |  | 
6|`password` | varchar |  |  | bcrypt hash of user password
7|`created_at` | timestamp |  |  | 
8|`updated_at` | timestamp |  |  | 
9|`deleted_at` | timestamp |  |  | 
10|`invalid_login_amount` | integer |  |  | 
11|`two_factor_secret_key` | varchar |  |  | 
12|`is_second_factor_passed` | boolean |  |  | 
13|`last_active` | timestamp |  |  | 
14|`phone_number` | varchar |  |  | 
15|`phone_number_prefix` | varchar |  |  | 
16|`phone_number_country_code` | varchar |  |  | 
