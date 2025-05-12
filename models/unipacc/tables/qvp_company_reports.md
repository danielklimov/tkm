qvp_company_reports
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | autogen
2|`company_id` | uuid |  | [`qvp_companies`](qvp_companies.md) | QVP service provider company
2|`qvp_company_id` | uuid |  | [`qvp_companies`](qvp_companies.md) | QVP service provider company
3|`report_status` | varchar |  |  | Status of the report. One of: accepted, waiting.
4|`file_id` | varchar |  | [`file_storage`](file_storage.md) | A reference to file_storage table.
5|`invoice_id` | uuid |  | [`qvp_company_invoices`](qvp_company_invoices.md) | An invoice that this report is attached to.
6|`created_at` | timestamp |  |  | 
7|`updated_at` | timestamp |  |  | 
8|`deleted_status` | varchar |  |  | ACTIVE, DELETED
23|`dasdasd` | asdas | dasda | [`dasd`](dasd.md) | 
