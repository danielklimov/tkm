
verification_request_certificates
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION  | COMMENTS          
---|------|-----------|----|----|--------------|----------
1|`id` | uuid | V |  |  | 
2|`verification_request_id` | uuid |  | [`verification_requests`](verification_requests.md) |  | 
3|`certificate_file` | varchar |  | [`file_storage`](file_storage.md) | A copy of the certificate document in pdf format | 
4|`first_name` | varchar |  |  | First name as spelled in the certificate document | 
5|`last_name` | varchar |  |  | Last name as spelled in the certificate document | 
6|`nationality` | varchar |  |  | A string, sometimes a country name, like 'Egypt', sometimes - a nationality name, like 'Belgian', as written in the certificate | 
7|`passport_number` | varchar |  |  | Passport number of a person the certificate is issued to. | 
8|`major_name` | varchar |  |  | Major (specialization) as it is set in the certificate | 
9|`created_at` | timestamp |  |  |  | 
10|`updated_at` | timestamp |  |  |  | 
11|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record. | 
