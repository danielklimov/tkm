verification_request_verification_types
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | autogen
2|`verification_request_id` | uuid |  | [`verification_requests`](verification_requests.md) | Verification request that requires this verification type
3|`verification_type` | varchar |  |  | Verification type. Enum. One of: EDUCATION,PROFESSIONAL_CERTIFICATE,EXPERIENCE
4|`created_at` | timestamp |  |  | 
5|`updated_at` | timestamp |  |  | 
6|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record.
