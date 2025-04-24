verification_request_personas
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | 
2|`first_name` | varchar |  |  | 
3|`last_name` | varchar |  |  | 
4|`middle_name` | varchar |  |  | Middle name or father's name
5|`gender` | varchar |  |  | One of: 'Female', 'Male'
6|`date_of_birth` | date |  |  | 
7|`nationality_id` | uuid |  | [`countries`](countries.md) | Country of nationality (citizenship).
8|`passport_id` | uuid |  | [`passport`](passport.md) | User's current passport.
9|`country_of_residence_id` | uuid |  | [`countries`](countries.md) | User's current country of residence (location).
10|`state_province` | varchar |  |  | State or province of current location (residence?)
11|`created_at` | timestamp |  |  | 
12|`updated_at` | timestamp |  |  | 
13|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record.
