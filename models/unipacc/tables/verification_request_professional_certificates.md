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
11|`verification_status` | varchar |  |  | One of: DRAFT, PENDING, IN_PROGRESS, FOR_UPDATE, UPDATED, ON_HOLD, VERIFIED, UNABLE_TO_VERIFY, REJECTED, WITHDRAWN
12|`verification_reject_reason_id` | uuid |  | [`verification_reject_reasons`](verification_reject_reasons.md) | Nullable. When verification_status is REJECTED or UNABLE_TO_VERIFY, a reject reason is required.
13|`verification_reject_comment` | varchar |  |  | If verification_reject_reason_id is set and it requires comment, the comment is specified here.
14|`verifier_user_id` | varchar |  | [`users`](users.md) | User account that was used by the verifier (qvp_company_employee)
15|`appeal_count` | integer |  |  | Total number of appeals
16|`first_verification_at` | timestamp |  |  | Same as 'end_verification_at' when verification is done for the first time.
17|`second_verification_at` | timestamp |  |  | Same as 'end_verification_at' when verification is done for the second time.
18|`start_verification_at` | timestamp |  |  | Date and time when verification started - verificaton_status became PENDING
19|`end_verification_at` | timestamp |  |  | Date and time when verification finished - verification_status became one of: VERIFIED, UNABLE_TO_VERIFY, REJECTED, WITHDRAWN
20|`sla_days_in_progress` | integer |  |  | Statistics: total days in progress
20|`sla_days_count` | integer |  |  | Number of days that this vr is in verification - from setting PENDING status to setting one of the final statuses: VERIFIED, UNABLE_TO_VERIFY, REJECTED. This attribute is recalculated daily
21|`sla_days_on_hold` | integer |  |  | 
21|`issuer_name` | varchar |  |  | Organization that issued the certificate
22|`report_file_id` | varchar |  | [`file_storage`](file_storage.md) | Verification report - printable version in pdf format
23|`validation_id` | uuid |  | [`verification_request_validations`](verification_request_validations.md) | A reference to the most recent validation
24|`created_at` | timestamp |  |  | 
25|`updated_at` | timestamp |  |  | 
26|`deleted_status` | varchar |  |  | ACTIVE, DELETED
