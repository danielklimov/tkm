qvp_company_sla_reports
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | autogen
2|`qvp_company_id` | uuid |  | [`qvp_companies`](qvp_companies.md) | 
3|`done_requests` | integer |  |  | Total number of completed verification requests
4|`average_days` | integer |  |  | Average days per verification of 1 verification request
5|`verification_request_type` | varchar |  |  | Type of verification request: 'education', 'experiene', 'professional certificate'. 
6|`created_at` | timestamp |  |  | 
7|`updated_at` | timestamp |  |  | 
8|`deleted_status` | varchar |  |  | ACTIVE, DELETED
