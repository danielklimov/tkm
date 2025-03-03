
qvp_company_invoices
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION  | COMMENTS          
---|------|-----------|----|----|--------------|----------
1|`id` | uuid | V |  | autogen | 
2|`message` | varchar |  |  | The message that is sent by SP to Takamol admin along with the invoice  | 
3|`file_id` | varchar |  | [`file_storage`](file_storage.md) | A printable version of the invoice | 
4|`invoice_status` | varchar |  |  | one of: not_sent, paid, payment_pending, returned, waiting | 
5|`created_at` | timestamp |  |  |  | 
6|`updated_at` | timestamp |  |  |  | 
7|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record. | 
19|`created_at` | timestamp |  |  |  | 
20|`updated_at` | timestamp |  |  |  | 
21|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record. | 
