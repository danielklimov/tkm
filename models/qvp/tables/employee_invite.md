
employee_invite
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | integer | V |  | 
2|`employee_id` | integer |  | [`service_provider_employee`](service_provider_employee.md) | 
3|`service_provider_id` | uuid |  | [`service_provider_company`](service_provider_company.md) | 
4|`token` | varchar |  |  | 
5|`email` | varchar |  |  | 
7|`expire_at` | timestamp |  |  | 
8|`created_at` | timestamp |  |  | 
9|`deleted_at` | timestamp |  |  | 
10|`verification_types` | json |  |  | 
