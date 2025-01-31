
service_provider_employee
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | integer | V |  | 
2|`user_id` | uuid |  | [`users`](users.md) | 
3|`company_id` | uuid |  | [`service_provider_company`](service_provider_company.md) | 
4|`deleted_at` | timestamp |  |  | 
