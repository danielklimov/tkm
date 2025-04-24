occupation_relevant_professional_certificates
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | Surrogate key
2|`occupation_id` | uuid |  | [`occupations`](occupations.md) | 
3|`professional_certificate_id` | uuid |  | [`professional_certificates`](professional_certificates.md) | 
4|`created_at` | timestamp |  |  | 
5|`updated_at` | timestamp |  |  | 
6|`deleted_status` | varchar |  |  | ACTIVE, DELETED
