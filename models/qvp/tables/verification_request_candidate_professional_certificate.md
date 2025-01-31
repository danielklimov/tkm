
verification_request_candidate_professional_certificate
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | uuid | V |  | 
3|`sla_hold` | uuid |  | [`verification_request_sla_holds`](verification_request_sla_holds.md) | 
4|`professional_certificate_id` | integer |  | [`professional_certificate`](professional_certificate.md) | 
6|`service_provider_employee_id` | integer |  | [`service_provider_employee`](service_provider_employee.md) | 
7|`service_provider_id` | uuid |  | [`service_provider_company`](service_provider_company.md) | 
8|`file_id` | varchar |  |  | 
9|`issued_date` | date |  |  | 
10|`expiry_date` | date |  |  | 
11|`institute_website` | varchar |  |  | 
12|`serial_no` | varchar |  |  | 
13|`status` | varchar |  |  | 
14|`verifier_user_id` | varchar |  |  | 
15|`appeal_count` | integer |  |  | 
16|`first_verification_at` | timestamp |  |  | 
17|`start_verification_at` | timestamp |  |  | 
18|`end_verification_at` | timestamp |  |  | 
19|`sla_days_in_progress` | integer |  |  | 
20|`sla_days_on_hold` | integer |  |  | 
21|`created_at` | timestamp |  |  | 
22|`updated_at` | timestamp |  |  | 
23|`deleted_at` | timestamp |  |  | 
24|`issuer_name` | varchar |  |  | 
26|`report_file_id` | varchar |  |  | 
27|`validation_id` | uuid |  |  | 
