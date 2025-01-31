
invoices
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | bigint | V |  | 
2|`payment_id` | bigint |  | [`payments`](payments.md) | 
3|`invoice_to` | varchar |  |  | 
4|`transaction_date` | timestamp |  |  | 
5|`reference_number` | varchar |  |  | 
6|`reference_method` | varchar |  |  | 
7|`total_amount` | money |  |  | 
8|`created_at` | timestamp |  |  | 
9|`updated_at` | timestamp |  |  | 
10|`withdrawal_id` | bigint |  | [`withdrawals`](withdrawals.md) | 
11|`qr_code` | text |  |  | 
12|`signed_einvoice` | text |  |  | 
13|`uuid` | varchar |  |  | 
15|`zatca_status` | integer |  |  | 
