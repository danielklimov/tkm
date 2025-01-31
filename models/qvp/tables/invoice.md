
invoice
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | uuid | V |  | 
2|`payment_transaction_id` | uuid |  | [`verification_payment_transaction`](verification_payment_transaction.md) | 
3|`file_id` | varchar |  |  | 
4|`number` | integer |  |  | 
6|`amount` | integer |  |  | 
7|`currency` | varchar |  |  | 
8|`type` | varchar |  |  | 
9|`brand` | varchar |  |  | 
10|`created_at` | timestamp |  |  | 
11|`deleted_at` | timestamp |  |  | 
12|`total_tax` | integer |  |  | 
13|`buyer_name` | varchar |  |  | 
14|`reference_number` | varchar |  |  | 
15|`reference_method` | varchar |  |  | 
16|`qr_code` | text |  |  | 
17|`supplier_tax_id` | varchar |  |  | 
18|`supplier_name` | varchar |  |  | 
19|`supplier_street` | varchar |  |  | 
20|`supplier_location` | varchar |  |  | 
21|`discount_amount` | integer |  |  | 
22|`currency_convert_ratio` | double precision |  |  | 
23|`payment_at` | timestamp |  |  | 
24|`positions` | text |  |  | 
25|`zatca_report` | text |  |  | 
