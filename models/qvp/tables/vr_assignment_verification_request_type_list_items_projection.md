
vr_assignment_verification_request_type_list_items_projection
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | uuid | V |  | 
2|`verification_request_id` | varchar |  |  | 
3|`verification_request_random_id` | varchar |  |  | 
4|`verification_request_created_date` | timestamp with time zone |  |  | 
5|`verification_request_updated_date` | timestamp with time zone |  |  | 
6|`verification_request_received_date` | timestamp with time zone |  |  | 
7|`verification_request_is_fast_track` | boolean |  |  | 
8|`verification_request_type_id` | varchar |  |  | 
9|`verification_request_type` | varchar |  |  | 
10|`verification_request_type_status` | varchar |  |  | 
11|`verification_request_type_sla_days_in_progress` | integer |  |  | 
12|`verification_request_type_appeal_available` | boolean |  |  | 
13|`submitter_nationality` | varchar |  |  | 
14|`submitter_current_location` | varchar |  |  | 
15|`submitter_first_name` | varchar |  |  | 
16|`submitter_second_name` | varchar |  |  | 
17|`submitter_last_name` | varchar |  |  | 
18|`submitter_passport_number` | varchar |  |  | 
19|`service_provider_company_name` | varchar |  |  | 
20|`service_provider_company_id` | varchar |  |  | 
21|`verifier_role` | varchar |  |  | 
22|`verifier_user_id` | varchar |  |  | 
23|`payment_status` | varchar |  |  | 
24|`education_major_status_check` | varchar |  |  | 
25|`education_level_status_check` | varchar |  |  | 
26|`occupation_name_english` | varchar |  |  | 
27|`occupation_name_arabic` | varchar |  |  | 
