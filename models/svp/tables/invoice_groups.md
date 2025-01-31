
invoice_groups
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | bigint | V |  | 
2|`service_description` | varchar |  |  | 
3|`unit_price` | integer |  |  | 
4|`quantity` | integer |  |  | 
5|`total_amount` | money |  |  | 
6|`invoice_id` | bigint |  | [`invoices`](invoices.md) | 
7|`created_at` | timestamp |  |  | 
8|`updated_at` | timestamp |  |  | 
