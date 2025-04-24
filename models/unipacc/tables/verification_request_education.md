verification_request_education
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | 
2|`education_level_id` | uuid |  | [`education_levels`](education_levels.md) | One of: Diploma, Bachelor, Masters, Doctoral
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
22|`verification_status` | varchar |  |  | One of: DRAFT, PENDING, IN_PROGRESS, FOR_UPDATE, UPDATED, ON_HOLD, VERIFIED, UNABLE_TO_VERIFY, REJECTED, WITHDRAWN
23|`verification_reject_reason_id` | uuid |  | [`verification_reject_reasons`](verification_reject_reasons.md) | Nullable. When verification_status is REJECTED or UNABLE_TO_VERIFY, a reject reason is required.
24|`verification_reject_comment` | varchar |  |  | If verification_reject_reason_id is set and it requires comment, the comment is specified here.
25|`verification_request_id` | uuid |  | [`verification_requests`](verification_requests.md) | TODO: Verification request that this record is connected to. There is a reverse reference - from verification_request to this table. Cardinality - 1:1 Remove this field?
26|`qvp_company_id` | uuid |  | [`qvp_companies`](qvp_companies.md) | The company that is assigned to verify this request
27|`qvp_company_employee_id` | uuid |  | [`qvp_company_employees`](qvp_company_employees.md) | QVP company employee assigned to this request
28|`appeal_count` | integer |  |  | Count of appeals. An 'appeal' is when the applicant appeals to verify education again after an unsuccessful attempt.
29|`first_verification_at` | timestamp |  |  | Same as 'end_verification_at' when verification is done for the first time.
30|`second_verification_at` | timestamp |  |  | Same as 'end_verification_at' when verification is done for the second time.
31|`start_verification_at` | timestamp |  |  | Date and time when verification started
32|`end_verification_at` | timestamp |  |  | Date and time when verification finished
33|`sla_hold` | uuid |  | [`verification_request_sla_holds`](verification_request_sla_holds.md) | description of a hold if one exists for this verification
34|`sla_days_in_progress` | integer |  |  | recalculated and updated every day
35|`sla_days_on_hold` | integer |  |  | recalculated and updated every day
36|`verifier_user_id` | uuid |  | [`users`](users.md) | The user that was doing the verification
37|`education_institute_place_id` | varchar |  |  | Google places Place id if applicable
38|`education_institute_id` | varchar |  | [`education_institutes`](education_institutes.md) | Matching education institute
39|`report_file_id` | varchar |  | [`file_storage`](file_storage.md) | verification report
40|`validation_id` | uuid |  | [`verification_request_validations`](verification_request_validations.md) | Reference to the most recent validation object - details of validation of this request. There can be more than 1 validation per request. This field points to the most recent one.
41|`exclude_from_already_verified` | boolean |  |  | TODO: does it mean that this request should be excluded from already verified and verified once more? Old field?
42|`education_certificate_file_id` | uuid |  | [`file_storage`](file_storage.md) | Attachment - education certificate
43|`education_transcript_file_id` | uuid |  | [`file_storage`](file_storage.md) | Attachment - transcript
44|`created_at` | timestamp |  |  | 
45|`updated_at` | timestamp |  |  | 
46|`deleted_status` | varchar |  |  | ACTIVE, DELETED
