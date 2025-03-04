verification_request_education
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION  | COMMENTS          
---|------|-----------|----|----|--------------|----------
1|`id` | uuid | V |  | 
2|`education_level` | varchar |  |  | One of: Diploma, Bachelor, Masters, Doctoral
3|`education_institute` | varchar |  |  | Name of education institute
4|`college` | varchar |  |  | Name of the college
5|`name_record` | varchar |  |  | Aplicant (former student) name as it is written in the educ. certificate
6|`major_name` | varchar |  |  | Major (specialization)
7|`start_date_enrollment` | timestamp |  |  | 
8|`end_date_enrollment` | timestamp |  |  | 
9|`institute_street` | varchar |  |  | 
10|`institute_building_number` | varchar |  |  | 
11|`institute_city` | varchar |  |  | 
12|`institute_state` | varchar |  |  | 
13|`institute_postal_code` | varchar |  |  | 
14|`institute_country` | varchar |  |  | 
15|`institute_phone_number` | varchar |  |  | 
16|`institute_web_address` | varchar |  |  | 
17|`student_id` | varchar |  |  | Institute's internal student id
18|`student_email` | varchar |  |  | 
19|`major_id` | uuid |  | [`majors`](majors.md) | A Major from internal list of majors that has been mapped to this edu. cert. 
20|`education_level_status_check` | varchar |  |  | one of: Incompatible, Compatible, Unable to verify
21|`institute_phone_number_country_code` | uuid |  | [`phone_country_codes`](phone_country_codes.md) | Institute phone country code
22|`status` | varchar |  |  | One of: payment_pending, updated, withdrawn, unpaid, unable_to_verify, returned, on_hold, rejected, drafted, pending, in_progress, accepted
23|`verification_request_id` | uuid |  | [`verification_requests`](verification_requests.md) | TODO: Verification request that this record is connected to. There is a reverse reference - from verification_request to this table. Cardinality - 1:1 Remove this field?
24|`qvp_company_id` | uuid |  | [`qvp_companies`](qvp_companies.md) | The company that is assigned to verify this request
25|`qvp_company_employee_id` | uuid |  | [`qvp_company_employees`](qvp_company_employees.md) | QVP company employee assigned to this request
26|`appeal_count` | integer |  |  | Count of appeals. An 'appeal' is when the applicant appeals to verify education again after an unsuccessful attempt.
27|`first_verification_at` | timestamp |  |  | TODO: what is first verification? First attempt to call the institute? Or there can be multiple verifications for a single verification request?
28|`start_verification_at` | timestamp |  |  | 
29|`end_verification_at` | timestamp |  |  | 
30|`sla_hold` | uuid |  | [`verification_request_sla_holds`](verification_request_sla_holds.md) | description of a hold if one exists for this verification
31|`sla_days_in_progress` | integer |  |  | recalculated and updated every day
32|`sla_days_on_hold` | integer |  |  | recalculated and updated every day
33|`verifier_user_id` | uuid |  | [`users`](users.md) | The user that was doing the verification
34|`education_institute_place_id` | varchar |  |  | Google places Place id if applicable
35|`education_institute_id` | varchar |  | [`education_institutes`](education_institutes.md) | Matching education institute
36|`report_file_id` | varchar |  | [`file_storage`](file_storage.md) | verification report
37|`validation_id` | uuid |  | [`verification_request_validations`](verification_request_validations.md) | Reference to the most recent validation object - details of validation of this request. There can be more than 1 validation per request. This field points to the most recent one.
38|`exclude_from_already_verified` | boolean |  |  | TODO: does it mean that this request should be excluded from already verified and verified once more? Old field?
39|`education_certificate_file_id` | uuid |  | [`file_storage`](file_storage.md) | Attachment - education certificate
40|`education_transcript_file_id` | uuid |  | [`file_storage`](file_storage.md) | Attachment - transcript
41|`created_at` | timestamp |  |  | 
42|`updated_at` | timestamp |  |  | 
43|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record.
