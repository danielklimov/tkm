vr_verified_employment_experience
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`verification_request_id` | uuid | V | [`verification_requests`](verification_requests.md) | 
2|`employment_experience_id` | uuid | V | [`verification_request_employment`](verification_request_employment.md) | 
3|`created_at` | timestamp |  |  | 
4|`updated_at` | timestamp |  |  | 
5|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record.
