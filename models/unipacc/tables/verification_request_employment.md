
verification_request_employment
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION  | COMMENTS          
---|------|-----------|----|----|--------------|----------
1|`id` | uuid | V |  | autogen | 
2|`contract_expire_date` | timestamp |  |  |  | 
3|`employer_name` | varchar |  |  | Employer name | 
4|`occupation_name` | varchar |  |  | Occupation name as specified in the contract | 
5|`contract_job_title_ar` | varchar |  |  | Job title in Arabic | 
6|`contract_job_title_en` | varchar |  |  | Job title in English | 
7|`contract_type_id` | varchar |  |  | full time, internship | full time, internship
8|`occupation_id` | integer |  | [`occupations`](occupations.md) | An occupation from the list of occupations that matches occupation_name | 
9|`years_of_experience` | integer |  |  | Months of experience and years of experience means the same but there's a complicated calculation logic under the hood which uses months and years in different places, so instead of recalculating every time it is stored like this | 
10|`months_of_experience` | integer |  |  | Months of experience and years of experience means the same but there's a complicated calculation logic under the hood which uses months and years in different places, so instead of recalculating every time it is stored like this | 
11|`job_offer_file_id` | varchar |  | [`file_storage`](file_storage.md) |   | 
12|`employment_start_date` | date |  |  | TODO: pls clarify what 'join' means. | employment start date
13|`verification_status` | varchar |  |  | One of: Pending,In progress, For Update, Updated, On hold, Verified, Unable to verify, Rejected, Rejected, Withdrawn | 
14|`verification_request_id` | uuid |  | [`verification_requests`](verification_requests.md) |  | 
15|`qvp_company_id` | uuid |  | [`qvp_companies`](qvp_companies.md) | Service provider who does the verification | 
16|`qvp_company_employee_id` | integer |  | [`qvp_company_employees`](qvp_company_employees.md) | Service provider employee assigned for this verification | 
17|`appeal_count` | integer |  |  | Candidate can appeal requests in Rejected or Unable to verify statuses | 
18|`first_verification_at` | timestamp |  |  |  | 
19|`start_verification_at` | timestamp |  |  |  | 
20|`end_verification_at` | timestamp |  |  |  | 
21|`verifier_user_id` | uuid |  | [`users`](users.md) | User that did the verification. This must be the same user as assigned to qvp_company_employee_id | TODO: not needed?
22|`report_file_id` | varchar |  | [`file_storage`](file_storage.md) | uuid. a ref to a file containing the verification report | 
23|`created_at` | timestamp |  |  |  | 
24|`updated_at` | timestamp |  |  |  | 
25|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record. | 
