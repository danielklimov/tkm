verification_request_professional_certificates
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | autogen
2|`sla_hold_id` | uuid |  | [`verification_request_sla_holds`](verification_request_sla_holds.md) | A ref to the most recent sla hold that was caused by verification of this certificate
3|`professional_certificate_id` | uuid |  | [`professional_certificates`](professional_certificates.md) | A reference to the list of known professional certificates
4|`qvp_company_employee_id` | uuid |  | [`qvp_company_employees`](qvp_company_employees.md) | SP employee who is assigned for doing the verification
5|`qvp_company_id` | uuid |  | [`qvp_companies`](qvp_companies.md) | Service provider who is doing the verification
6|`file_id` | varchar |  | [`file_storage`](file_storage.md) | A copy of professional certificate in pdf format
7|`issued_date` | date |  |  | Certificate issue date
8|`expiry_date` | date |  |  | Certificate expiry date
9|`institute_website` | varchar |  |  | Website URL of the institute that issued the certificate
10|`serial_no` | varchar |  |  | Human-readable certificate number
11|`verification_status` | varchar |  |  | One of: payment_pending, updated, withdrawn, unpaid, unable_to_verify, returned, on_hold, rejected, drafted, pending, in_progress,accepted
12|`verifier_user_id` | varchar |  | [`users`](users.md) | User account that was used by the verifier (qvp_company_employee)
13|`appeal_count` | integer |  |  | Total number of appeals
14|`first_verification_at` | timestamp |  |  | 
15|`start_verification_at` | timestamp |  |  | 
16|`end_verification_at` | timestamp |  |  | 
17|`sla_days_in_progress` | integer |  |  | Statistics: total days in progress
18|`sla_days_on_hold` | integer |  |  | 
19|`issuer_name` | varchar |  |  | Organization that issued the certificate
20|`report_file_id` | varchar |  | [`file_storage`](file_storage.md) | Verification report - printable version in pdf format
21|`validation_id` | uuid |  | [`verification_request_validations`](verification_request_validations.md) | A reference to the most recent validation
22|`created_at` | timestamp |  |  | 
23|`updated_at` | timestamp |  |  | 
24|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record.
