
verification_payment_checkout
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | uuid | V |  | 
2|`verification_request` | uuid |  | [`verification_request`](verification_request.md) | 
3|`code` | varchar |  |  | 
4|`status` | varchar |  |  | 
5|`amount` | integer |  |  | 
6|`currency` | varchar |  |  | 
7|`payment_type` | varchar |  |  | 
8|`description` | varchar |  |  | 
9|`hyper_pay_checkout_id` | varchar |  |  | 
10|`created_at` | timestamp |  |  | 
11|`deleted_at` | timestamp |  |  | 
12|`total_tax` | integer |  |  | 
