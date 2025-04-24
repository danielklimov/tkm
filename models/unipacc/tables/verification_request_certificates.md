verification_request_certificates
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | 
2|`verification_request_id` | uuid |  | [`verification_requests`](verification_requests.md) | 
3|`certificate_number` | varchar(40) |  |  | Human-readable certificate number that is printed on the paper document.
4|`certificate_file` | varchar |  | [`file_storage`](file_storage.md) | A copy of the certificate document in pdf format
5|`first_name` | varchar |  |  | First name as spelled in the certificate document
6|`last_name` | varchar |  |  | Last name as spelled in the certificate document
7|`middle_name` | varchar |  |  | 
8|`nationality_id` | varchar |  | [`countries`](countries.md) | A string, sometimes a country name, like 'Egypt', sometimes - a nationality name, like 'Belgian', as written in the certificate
9|`passport_number` | varchar |  |  | Passport number of a person the certificate is issued to.
10|`occupation_id` | varchar |  | [`occupations`](occupations.md) | Occupation as it is set in the certificate
11|`created_at` | timestamp |  |  | 
12|`updated_at` | timestamp |  |  | 
13|`deleted_status` | varchar |  |  | ACTIVE, DELETED
