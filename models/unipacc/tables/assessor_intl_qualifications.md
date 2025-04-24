assessor_intl_qualifications
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | 
2|`assessor_id` | uuid |  | [`assessors`](assessors.md) | 
3|`intl_qualification_code` | varchar |  |  | One of: degree, diploma, training
4|`created_at` | timestamp |  |  | 
5|`updated_at` | timestamp |  |  | 
6|`deleted_status` | varchar |  |  | ACTIVE, DELETED
