
verification_request_education
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | uuid | V |  | 
2|`education_level` | varchar |  |  | 
3|`education_institute` | varchar |  |  | 
4|`college` | varchar |  |  | 
5|`name_record` | varchar |  |  | 
6|`major_name` | varchar |  |  | 
7|`grade_point_average` | varchar |  |  | 
8|`graduation_date` | timestamp |  |  | 
9|`start_date_enrollment` | timestamp |  |  | 
10|`end_date_enrollment` | timestamp |  |  | 
11|`institute_street` | varchar |  |  | 
12|`institute_building_number` | varchar |  |  | 
13|`institute_city` | varchar |  |  | 
14|`institute_state` | varchar |  |  | 
15|`institute_postal_code` | varchar |  |  | 
16|`institute_country` | varchar |  |  | 
17|`institute_phone_number` | varchar |  |  | 
18|`institute_web_address` | varchar |  |  | 
19|`deleted_at` | timestamp |  |  | 
20|`award_name` | varchar |  |  | 
21|`award_date` | timestamp |  |  | 
22|`student_id` | varchar |  |  | 
23|`student_email` | varchar |  |  | 
24|`major_id` | integer |  |  | 
25|`education_level_status_check` | varchar |  |  | 
26|`major_status_check` | varchar |  |  | 
27|`institute_phone_number_code` | varchar |  |  | 
28|`institute_phone_number_country_code` | varchar |  |  | 
29|`status` | varchar |  |  | 
30|`verification_request_id` | uuid |  | [`verification_request`](verification_request.md) | 
31|`service_provider_id` | uuid |  | [`service_provider_company`](service_provider_company.md) | 
32|`service_provider_employee_id` | integer |  | [`service_provider_employee`](service_provider_employee.md) | 
33|`appeal_count` | integer |  |  | 
34|`first_verification_at` | timestamp |  |  | 
35|`start_verification_at` | timestamp |  |  | 
36|`end_verification_at` | timestamp |  |  | 
37|`sla_hold` | uuid |  | [`verification_request_sla_holds`](verification_request_sla_holds.md) | 
38|`sla_days_in_progress` | integer |  |  | 
39|`sla_days_on_hold` | integer |  |  | 
40|`apostille_added` | boolean |  |  | 
41|`verifier_user_id` | uuid |  |  | 
42|`education_institute_place_id` | varchar |  |  | 
