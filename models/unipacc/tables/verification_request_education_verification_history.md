verification_request_education_verification_history
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | surrogate key
2|`vr_education_id` | uuid |  | [`verification_request_education`](verification_request_education.md) | 
3|`end_verification_at` | timestamp |  |  | Date and time when verification finished
4|`valid_from` | timestamp |  |  | Business date and time starting from which the data that this record contains is valid
5|`created_at` | timestamp |  |  | 
6|`updated_at` | timestamp |  |  | 
7|`deleted_status` | varchar |  |  | ACTIVE, DELETED
