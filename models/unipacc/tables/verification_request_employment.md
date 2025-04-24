verification_request_employment
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | autogen
2|`occupation_id` | uuid |  | [`occupations`](occupations.md) | An occupation from the list of occupations that matches occupation_name
3|`contract_type` | varchar |  |  | Enum: FULL_TIME, PART_TIME
4|`job_offer_file_id` | varchar |  | [`file_storage`](file_storage.md) | Experience or Clearance Certificate 
5|`employment_start_date` | date |  |  | employment start date
6|`employment_end_date` | date |  |  | 
7|`actual_years_count` | numeric(18,2) |  |  | actual working years calculated in accordance with US APPL-38
8|`employer_name` | varchar |  |  | Employer name
9|`employer_country_id` | uuid |  | [`countries`](countries.md) | Employment address: country
10|`employer_state_province` | varchar |  |  | Employment address: state/province
11|`employer_city` | varchar |  |  | Employment address: city
12|`employer_street` | varchar |  |  | Employment address: street
13|`employer_building` | varchar |  |  | Employment address: building
14|`employer_zip_code` | varchar |  |  | Employment address: zip code
15|`employer_email` | varchar |  |  | Employer's email
16|`employer_phone_country_code_id` | uuid |  | [`phone_country_codes`](phone_country_codes.md) | Employer's phone country code
17|`employer_phone` | varchar |  |  | Employer's phone number without country code
18|`employer_website_url` | varchar |  |  | Employer's website
19|`verification_status` | varchar |  |  | One of: DRAFT, PENDING, IN_PROGRESS, FOR_UPDATE, UPDATED, ON_HOLD, VERIFIED, UNABLE_TO_VERIFY, REJECTED, WITHDRAWN
20|`verification_reject_reason_id` | uuid |  | [`verification_reject_reasons`](verification_reject_reasons.md) | Nullable. When verification_status is REJECTED or UNABLE_TO_VERIFY, a reject reason is required.
21|`verification_reject_comment` | varchar |  |  | If verification_reject_reason_id is set and it requires comment, the comment is specified here.
22|`verification_request_id` | uuid |  | [`verification_requests`](verification_requests.md) | VR that this vr_employment is attached to
23|`qvp_company_id` | uuid |  | [`qvp_companies`](qvp_companies.md) | Service provider who does the verification
24|`qvp_company_employee_id` | integer |  | [`qvp_company_employees`](qvp_company_employees.md) | Service provider employee assigned for this verification
25|`appeal_count` | integer |  |  | Candidate can appeal requests in Rejected or Unable to verify statuses
26|`first_verification_at` | timestamp |  |  | Same as 'end_verification_at' when verification is done for the first time.
27|`second_verification_at` | timestamp |  |  | Same as 'end_verification_at' when verification is done for the second time.
28|`start_verification_at` | timestamp |  |  | 
29|`end_verification_at` | timestamp |  |  | 
30|`verifier_user_id` | uuid |  | [`users`](users.md) | User that did the verification. This must be the same user as assigned to qvp_company_employee_id
31|`report_file_id` | varchar |  | [`file_storage`](file_storage.md) | uuid. a ref to a file containing the verification report
32|`created_at` | timestamp |  |  | 
33|`updated_at` | timestamp |  |  | 
34|`deleted_status` | varchar |  |  | ACTIVE, DELETED
