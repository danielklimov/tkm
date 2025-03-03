
qvp_company_reports
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION  | COMMENTS          
---|------|-----------|----|----|--------------|----------
1|`id` | uuid | V |  | autogen | 
2|`company_id` | uuid |  | [`qvp_companies`](qvp_companies.md) | QVP service provider company | 
3|`report_status` | varchar |  |  | Status of the report. One of: accepted, waiting. | 
4|`file_id` | varchar |  | [`file_storage`](file_storage.md) | A reference to file_storage table. | 
5|`invoice_id` | uuid |  | [`qvp_company_invoices`](qvp_company_invoices.md) | An invoice that this report is attached to. | 
6|`created_at` | timestamp |  |  |  | 
7|`updated_at` | timestamp |  |  |  | 
8|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record. | 
20|`created_at` | timestamp |  |  |  | 
21|`updated_at` | timestamp |  |  |  | 
22|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record. | 
