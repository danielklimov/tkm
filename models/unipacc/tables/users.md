
users
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION  | COMMENTS          
---|------|-----------|----|----|--------------|----------
1|`email` | varchar |  |  | User's email used for logging in | 
2|`roles` | varchar[] |  |  | Roles | 
3|`first_name` | varchar |  |  |  | 
4|`last_name` | varchar |  |  |  | 
5|`phone_number` | varchar |  |  |  | 
6|`phone_country_id` | integer |  | [`countries`](countries.md) | Country code that the phone number is issued in (not the telephone country code itself). The telephone country code is looked up in countries table | 
7|`password` | varchar |  |  | password digest. | BCrypt method is used in QVP and SVP. It can be reused here
8|`last_active_at` | timestamp |  |  |  | 
9|`invalid_login_attempts` | integer |  |  |  | 
10|`two_factor_secret_key` | varchar |  |  |  | 2FA logic: The 2nd key is generated, saved to 'two_factor_secret_key'. When the user enters the correct key, the field 'is_second_factor_passed' is set to true. TODO: At which point does the system change values of these fields to a new 2nd key and 'false' ?
11|`is_second_factor_passed` | boolean |  |  |  | 
12|`created_at` | timestamp |  |  |  | 
13|`updated_at` | timestamp |  |  |  | 
14|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record. | 
