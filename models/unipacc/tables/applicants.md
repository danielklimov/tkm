applicants
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION  | COMMENTS          
---|------|-----------|----|----|--------------|----------
1|`applicant_id` | uuid | V |  | 
2|`user_id` | uuid |  | [`users`](users.md) | User account used by the applicant to log in
3|`gender` | varchar |  |  | One of: male, female
4|`date_of_birth` | date |  |  | 
5|`country_of_residence_id` | integer |  | [`countries`](countries.md) | Current country of residence
6|`phone_number` | varchar |  |  | Phone number without country code
7|`phone_country_code_id` | integer |  | [`phone_country_codes`](phone_country_codes.md) | Country id that the phone number is issued in (not the telephone country code itself).
8|`email` | varchar |  |  | Applicant's email.
9|`first_name` | varchar |  |  | 
10|`middle_name` | varchar |  |  | 
11|`last_name` | varchar |  |  | 
12|`maiden_name` | varchar |  |  | 
13|`former_married_name` | varchar |  |  | 
14|`mothers_name` | varchar |  |  | 
15|`suffix` | varchar |  |  | Suffix that goes after last_name, like Ph.D.
16|`passport_id` | uuid |  | [`passports`](passports.md) | Currently active passport. A historical attribute. When its value changes, old value is stored in applicants_passports table
17|`notification_lang` | varchar |  |  | Language, selected by user for receiving notifications - two-letter code. One of: en, ar
18|`ui_lang` | varchar |  |  | User interface language. One of: en, ar
19|`fast_track_record_id` | uuid |  | [`fast_track_immediate_record`](fast_track_immediate_record.md) | Reference to the fast track record that was created for this applicant
20|`is_auto_registered` | boolean |  |  | true if the record was created for this person automatically without the applicant interaction.
21|`created_at` | timestamp |  |  | 
22|`updated_at` | timestamp |  |  | 
23|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record.
