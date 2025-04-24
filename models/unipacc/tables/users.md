users
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | 
2|`email` | varchar |  |  | User's email used for logging in
3|`roles` | varchar[] |  |  | Roles
4|`first_name` | varchar |  |  | 
5|`last_name` | varchar |  |  | 
6|`phone_number` | varchar |  |  | 
7|`phone_country_code_id` | uuid |  | [`phone_country_codes`](phone_country_codes.md) | Phone country code
8|`password` | varchar |  |  | password digest.
9|`last_active_at` | timestamp |  |  | 
10|`invalid_login_attempts` | integer |  |  | 
11|`two_factor_secret_key` | varchar |  |  | 
12|`is_second_factor_passed` | boolean |  |  | 
13|`ui_lang` | varchar |  |  | User interface language. One of: en, ar
14|`notification_lang` | varchar |  |  | Language, selected by user for receiving notifications - two-letter code. One of: en, ar
15|`created_at` | timestamp |  |  | 
16|`updated_at` | timestamp |  |  | 
17|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record.
