
verification_request_type_list_items_projection
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
8|`verification_request_type` | varchar |  |  | 
9|`verification_request_type_id` | varchar |  |  | 
10|`verification_request_type_status` | varchar |  |  | 
11|`verification_request_type_sla_days_in_progress` | integer |  |  | 
12|`verification_request_type_sla_days_on_hold` | integer |  |  | 
13|`verification_request_type_on_hold_id` | varchar |  |  | 
14|`verification_request_type_appeal_available` | boolean |  |  | 
15|`service_provider_order_id` | varchar |  |  | 
16|`submitter_first_name` | varchar |  |  | 
17|`submitter_second_name` | varchar |  |  | 
18|`submitter_last_name` | varchar |  |  | 
19|`submitter_passport_number` | varchar |  |  | 
20|`submitter_nationality` | varchar |  |  | 
21|`submitter_country` | varchar |  |  | 
22|`education_major_status_check` | varchar |  |  | 
23|`education_level_status_check` | varchar |  |  | 
24|`education_has_apostille_certificate` | boolean |  |  | 
25|`service_provider_company_id` | uuid |  |  | 
26|`verifier_user_full_name` | varchar |  |  | 
27|`verifier_user_id` | uuid |  |  | 
