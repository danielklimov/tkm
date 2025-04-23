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
13|`grandfather_name` | varchar |  |  | Grandfather's name
14|`maiden_name` | varchar |  |  | 
15|`former_married_name` | varchar |  |  | 
16|`mothers_name` | varchar |  |  | 
17|`suffix` | varchar |  |  | Suffix that goes after last_name, like Ph.D.
18|`passport_id` | uuid |  | [`passports`](passports.md) | Currently active passport. A historical attribute. When its value changes, old value is stored in applicants_passports table
19|`notification_lang` | varchar |  |  | Language, selected by user for receiving notifications - two-letter code. One of: en, ar
20|`ui_lang` | varchar |  |  | User interface language. One of: en, ar
21|`fast_track_record_id` | uuid |  | [`fast_track_immediate_record`](fast_track_immediate_record.md) | Reference to the fast track record that was created for this applicant
22|`is_auto_registered` | boolean |  |  | true if the record was created for this person automatically without the applicant interaction.
23|`created_at` | timestamp |  |  | 
24|`updated_at` | timestamp |  |  | 
25|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record.
