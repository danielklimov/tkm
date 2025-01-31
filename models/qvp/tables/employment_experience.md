
employment_experience
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | uuid | V |  | 
2|`occupation_id` | integer |  | [`occupation`](occupation.md) | 
3|`country_id` | uuid |  | [`verification_request_nationality`](verification_request_nationality.md) | 
4|`institute_name` | varchar |  |  | 
5|`start_date` | timestamp |  |  | 
6|`end_date` | timestamp |  |  | 
7|`employment_type` | varchar |  |  | 
8|`state` | varchar |  |  | 
9|`city` | varchar |  |  | 
10|`street_name` | varchar |  |  | 
11|`building_number` | varchar |  |  | 
12|`zip_code` | varchar |  |  | 
13|`institute_phone_number` | varchar |  |  | 
14|`institute_website` | varchar |  |  | 
15|`institute_email` | varchar |  |  | 
16|`certificate_id` | varchar |  |  | 
18|`institute_phone_number_code` | varchar |  |  | 
19|`institute_phone_number_country_code` | varchar |  |  | 
20|`created_at` | timestamp |  |  | 
21|`verification_request_id` | uuid |  | [`verification_request`](verification_request.md) | 
22|`sla_hold` | uuid |  | [`verification_request_sla_holds`](verification_request_sla_holds.md) | 
23|`service_provider_employee_id` | integer |  | [`service_provider_employee`](service_provider_employee.md) | 
24|`service_provider_id` | uuid |  | [`service_provider_company`](service_provider_company.md) | 
25|`status` | varchar |  |  | 
26|`verifier_user_id` | varchar |  |  | 
27|`appeal_count` | integer |  |  | 
28|`first_verification_at` | timestamp |  |  | 
29|`start_verification_at` | timestamp |  |  | 
30|`end_verification_at` | timestamp |  |  | 
31|`sla_days_in_progress` | integer |  |  | 
32|`sla_days_on_hold` | integer |  |  | 
33|`updated_at` | timestamp |  |  | 
34|`deleted_at` | timestamp |  |  | 
35|`report_file_id` | varchar |  |  | 
36|`validation_id` | uuid |  |  | 
