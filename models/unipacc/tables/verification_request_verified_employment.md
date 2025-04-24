verification_request_verified_employment
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` |  | V |  | surrogate key
2|`verification_request_id` | uuid |  | [`verification_requests`](verification_requests.md) | 
3|`employment_experience_id` | uuid |  | [`verification_request_employment`](verification_request_employment.md) | 
4|`created_at` | timestamp |  |  | 
5|`updated_at` | timestamp |  |  | 
6|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record.
