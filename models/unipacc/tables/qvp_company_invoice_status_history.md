qvp_company_invoice_status_history
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION  | COMMENTS          
---|------|-----------|----|----|--------------|----------
1|`id` | uuid | V |  | autoinc
2|`invoice_id` | uuid |  | [`qvp_company_invoices`](qvp_company_invoices.md) | 
3|`invoice_status` | varchar |  |  | one of: not_sent, paid, payment_pending, returned, waiting.
4|`valid_from` | timestamp |  |  | Date and time when invoice_status became valid
5|`created_at` | timestamp |  |  | 
6|`updated_at` | timestamp |  |  | 
7|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record.
19|`created_at` | timestamp |  |  | 
20|`updated_at` | timestamp |  |  | 
21|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record.
