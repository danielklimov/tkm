qvp_company_employee_reports
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | 
2|`qvp_company_employee_id` | integer |  | [`qvp_company_employees`](qvp_company_employees.md) | 
3|`report_file_id` | uuid |  |  | TODO: it isn't referencing file_storage!
4|`created_at` | timestamp |  |  | 
5|`updated_at` | timestamp |  |  | 
6|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record.
18|`created_at` | timestamp |  |  | 
19|`updated_at` | timestamp |  |  | 
20|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record.
