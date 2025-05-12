qvp_certificates
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | 
2|`applicant_id` | uuid |  | [`applicants`](applicants.md) | The applicant that applied for the certificate.
3|`certificate_number` | varchar(40) |  |  | Human-readable certificate number that is printed on the paper document.
4|`certificate_file_id` | uuid |  | [`file_storage`](file_storage.md) | A copy of the certificate document in pdf format. File type: QVP_CERTIFICATE
5|`first_name` | varchar |  |  | First name as spelled in the certificate document
6|`last_name` | varchar |  |  | Last name as spelled in the certificate document
7|`middle_name` | varchar |  |  | 
8|`nationality_id` | uuid |  | [`countries`](countries.md) | Reference to the country of citizenship (nationality) of the applicant at the time when the certificate was issued
9|`passport_number` | varchar |  |  | Passport number of a person that the certificate is issued to.
10|`occupation_id` | varchar |  | [`occupations`](occupations.md) | Occupation that is being certified
11|`verification_request_id` | uuid |  | [`verification_requests`](verification_requests.md) | The certificate was created as the result of processing this verification request
12|`created_at` | timestamp |  |  | 
13|`updated_at` | timestamp |  |  | 
14|`deleted_status` | varchar |  |  | ACTIVE, DELETED
