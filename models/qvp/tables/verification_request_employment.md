
verification_request_employment
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | uuid | V |  | 
6|`contract_expire_date` | timestamp |  |  | 
8|`establishment_name` | varchar |  |  | 
9|`deleted_at` | timestamp |  |  | 
11|`contract_status` | varchar |  |  | 
12|`occupation_name` | varchar |  |  | 
13|`occupation_key` | varchar |  |  | 
14|`contract_id` | varchar |  |  | 
15|`contract_job_title_ar` | varchar |  |  | 
16|`contract_job_title_en` | varchar |  |  | 
17|`contract_type_name` | varchar |  |  | 
18|`contract_type_id` | varchar |  |  | 
19|`establishment_id` | varchar |  |  | 
20|`establishment_entity_id` | varchar |  |  | 
21|`establishment_labor_office_id` | varchar |  |  | 
22|`establishment_unified_number_id` | varchar |  |  | 
23|`establishment_email` | varchar |  |  | 
24|`updated_at` | timestamp |  |  | 
25|`establishment_sequence_number` | varchar |  |  | 
26|`occupation_id` | integer |  |  | 
27|`years_of_experience` | integer |  |  | 
28|`job_offer_file_id` | varchar |  |  | 
29|`status` | varchar |  |  | 
30|`verification_request_id` | uuid |  | [`verification_request`](verification_request.md) | 
31|`service_provider_id` | uuid |  | [`service_provider_company`](service_provider_company.md) | 
32|`service_provider_employee_id` | integer |  | [`service_provider_employee`](service_provider_employee.md) | 
33|`appeal_count` | integer |  |  | 
34|`first_verification_at` | timestamp |  |  | 
35|`start_verification_at` | timestamp |  |  | 
36|`end_verification_at` | timestamp |  |  | 
37|`verifier_user_id` | uuid |  |  | 
38|`months_of_experience` | integer |  |  | 
