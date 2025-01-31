
report
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | integer | V |  | 
2|`company_id` | uuid |  | [`service_provider_company`](service_provider_company.md) | 
3|`uuid` | uuid |  |  | 
6|`status` | varchar |  |  | 
7|`created_at` | timestamp |  |  | 
8|`file_id` | varchar |  |  | 
9|`invoice_id` | integer |  | [`service_provider_company_invoice`](service_provider_company_invoice.md) | 
