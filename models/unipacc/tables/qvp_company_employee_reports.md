qvp_company_employee_reports
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | 
2|`qvp_company_employee_id` | integer |  | [`qvp_company_employees`](qvp_company_employees.md) | 
3|`report_file_id` | uuid |  | [`file_storage`](file_storage.md) | TODO: it isn't referencing file_storage in stg v2 db! An error?
4|`created_at` | timestamp |  |  | 
4|`created_at` | timestamp |  |  | 
5|`updated_at` | timestamp |  |  | 
5|`updated_at` | timestamp |  |  | 
6|`deleted_status` | varchar |  |  | ACTIVE, DELETED
6|`deleted_status` | varchar |  |  | ACTIVE, DELETED
