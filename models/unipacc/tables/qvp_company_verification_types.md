qvp_company_verification_types
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | autogen
2|`qvp_company_id` | uuid |  | [`qvp_companies`](qvp_companies.md) | 
3|`verification_type` | varchar |  |  | Verification type. Enum. One of: EDUCATION,PROFESSIONAL_CERTIFICATE,EXPERIENCE
4|`created_at` | timestamp |  |  | 
5|`updated_at` | timestamp |  |  | 
6|`deleted_status` | varchar |  |  | ACTIVE, DELETED
