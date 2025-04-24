applicants
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`applicant_id` | uuid | V |  | 
2|`user_id` | uuid |  | [`users`](users.md) | User account used by the applicant to log in
3|`gender` | varchar |  |  | One of: male, female
4|`date_of_birth` | date |  |  | 
5|`country_of_residence_id` | integer |  | [`countries`](countries.md) | Current country of residence
6|`state_province` | varchar |  |  | State or province of current location (residence?)
7|`phone_number` | varchar |  |  | Phone number without country code
8|`phone_country_code_id` | integer |  | [`phone_country_codes`](phone_country_codes.md) | Country id that the phone number is issued in (not the telephone country code itself).
9|`email` | varchar |  |  | Applicant's email.
10|`first_name` | varchar |  |  | 
11|`middle_name` | varchar |  |  | Middle name or father's name
12|`last_name` | varchar |  |  | 
13|`maiden_name` | varchar |  |  | 
14|`former_married_name` | varchar |  |  | 
15|`mothers_name` | varchar |  |  | 
16|`suffix` | varchar |  |  | Suffix that goes after last_name, like Ph.D.
17|`passport_id` | uuid |  | [`passports`](passports.md) | Currently active passport. A historical attribute. When its value changes, old value is stored in applicant_passport_history table
18|`fast_track_record_id` | uuid |  | [`fast_track_immediate_record`](fast_track_immediate_record.md) | Reference to the fast track record that was created for this applicant
19|`is_auto_registered` | boolean |  |  | true if the record was created for this person automatically without the applicant interaction.
20|`created_at` | timestamp |  |  | 
21|`updated_at` | timestamp |  |  | 
22|`deleted_status` | varchar |  |  | ACTIVE, DELETED
