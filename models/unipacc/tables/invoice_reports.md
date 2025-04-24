invoice_reports
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | autoincrement
2|`hyper_pay_payment_id` | varchar |  |  | HyperPay internal payment id
3|`status` | varchar |  |  | payment status: on of: PENDING, SUCCEEDED
4|`created_at` | timestamp |  |  | 
5|`invoice_type` | varchar |  |  | So far all records contain one value - 'invoice'. Lets keep it. Although RN we only have invoices for VRs, later we might have sub-invoices for extra payments, this is where we'll be able to specify types
6|`created_at` | timestamp |  |  | 
7|`updated_at` | timestamp |  |  | 
8|`deleted_status` | varchar |  |  | ACTIVE, DELETED
