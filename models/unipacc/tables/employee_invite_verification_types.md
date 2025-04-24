employee_invite_verification_types
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | 
2|`employee_invite_id` | uuid |  | [`employee_invites`](employee_invites.md) | 
3|`verification_type` | varchar |  |  | One of: "professionalCertificate", "education", "experience"
4|`created_at` | timestamp |  |  | 
5|`updated_at` | timestamp |  |  | 
6|`deleted_status` | varchar |  |  | ACTIVE, DELETED
