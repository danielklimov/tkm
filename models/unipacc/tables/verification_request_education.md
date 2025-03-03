
verification_request_education
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION  | COMMENTS          
---|------|-----------|----|----|--------------|----------
1|`id` | uuid | V |  |  | 
2|`education_level` | varchar |  |  | One of: Diploma, Bachelor, Masters, Doctoral | 
3|`education_institute` | varchar |  |  | Name of education institute | 
4|`college` | varchar |  |  | College if aplicable | 
5|`name_record` | varchar |  |  | Aplicant (former student) name as it is written in the educ. certificate | 
6|`major_name` | varchar |  |  | Major (specialization) | 
7|`grade_point_average` | varchar |  |  |  | 
8|`graduation_date` | timestamp |  |  |  | 
9|`start_date_enrollment` | timestamp |  |  |  | 
10|`end_date_enrollment` | timestamp |  |  |  | 
11|`institute_street` | varchar |  |  |  | 
12|`institute_building_number` | varchar |  |  |  | 
13|`institute_city` | varchar |  |  |  | 
14|`institute_state` | varchar |  |  |  | 
15|`institute_postal_code` | varchar |  |  |  | 
16|`institute_country` | varchar |  |  |  | 
17|`institute_phone_number` | varchar |  |  |  | 
18|`institute_web_address` | varchar |  |  |  | 
19|`award_name` | varchar |  |  |  | 
20|`award_date` | timestamp |  |  |  | 
21|`student_id` | varchar |  |  | Institute's internal student id | 
22|`student_email` | varchar |  |  |  | 
23|`major_id` | uuid |  | [`majors`](majors.md) | A Major from internal list of majors that has been mapped to this edu. cert.  | 
24|`education_level_status_check` | varchar |  |  | one of: Incompatible, Compatible, Unable to verify | 
25|`major_status_check` | varchar |  |  | one of: Incompatible, Compatible, Unable to verify | 
26|`institute_phone_number_country_code` | uuid |  | [`phone_country_codes`](phone_country_codes.md) | Institute phone country code | 
27|`status` | varchar |  |  | One of: payment_pending, updated, withdrawn, unpaid, unable_to_verify, returned, on_hold, rejected, drafted, pending, in_progress, accepted | 
28|`verification_request_id` | uuid |  | [`verification_requests`](verification_requests.md) | TODO: Verification request that this record is connected to. There is a reverse reference - from verification_request to this table. Cardinality - 1:1 Remove this field? | 
29|`qvp_company_id` | uuid |  | [`qvp_companies`](qvp_companies.md) | The company that is assigned to verify this request | 
30|`qvp_company_employee_id` | uuid |  | [`qvp_company_employees`](qvp_company_employees.md) | QVP company employee assigned to this request | 
31|`appeal_count` | integer |  |  | Count of appeals. An 'appeal' is when the applicant appeals to verify education again after an unsuccessful attempt. | 
32|`first_verification_at` | timestamp |  |  | TODO: what is first verification? First attempt to call the institute? Or there can be multiple verifications for a single verification request? | No idea
33|`start_verification_at` | timestamp |  |  |  | 
34|`end_verification_at` | timestamp |  |  |  | 
35|`sla_hold` | uuid |  | [`verification_request_sla_holds`](verification_request_sla_holds.md) | description of a hold if one exists for this verification | circular reference: vr_sla_holds->vr_sla_logs->vr_education. TODO: delete?
36|`sla_days_in_progress` | integer |  |  | recalculated and updated every day | 
37|`sla_days_on_hold` | integer |  |  | recalculated and updated every day | 
38|`is_apostille_added` | boolean |  |  | The education certificate/diploma has an apostille | 
39|`verifier_user_id` | uuid |  | [`users`](users.md) | The user that was doing the verification | 
40|`education_institute_place_id` | varchar |  |  | Google places Place id if applicable | 
41|`education_institute_id` | varchar |  | [`education_institutes`](education_institutes.md) | Matching education institute | 
42|`report_file_id` | varchar |  | [`file_storage`](file_storage.md) | verification report | 
43|`validation_id` | uuid |  | [`verification_request_validations`](verification_request_validations.md) | Reference to the most recent validation object - details of validation of this request. There can be more than 1 validation per request. This field points to the most recent one. | TODO: In QVP there are 2 separate entities - 'validation' and 'validation_history'. Here I have merged them into one - validation_history. Validation entity in QVP has 'previous_invalid_fields' field. Probably we should create a field here called 'prev_vr_validation' to reference the previous validation
44|`exclude_from_already_verified` | boolean |  |  | TODO: does it mean that this request should be excluded from already verified and verified once more? Old field? | Seem strange to me, we never had such a functionality
45|`education_certificate_file_id` | uuid |  | [`file_storage`](file_storage.md) | Attachment - education certificate | 
46|`education_transcript_file_id` | uuid |  | [`file_storage`](file_storage.md) | Attachment - transcript | 
47|`created_at` | timestamp |  |  |  | 
48|`updated_at` | timestamp |  |  |  | 
49|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record. | 
