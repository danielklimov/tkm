
verification_payment_transaction
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | uuid | V |  | 
2|`verification_request_id` | uuid |  | [`verification_request`](verification_request.md) | 
3|`hyper_pay_payment_id` | varchar |  |  | 
5|`status` | varchar |  |  | 
6|`email` | varchar |  |  | 
7|`description` | varchar |  |  | 
8|`payment_brand` | varchar |  |  | 
9|`payment_type` | varchar |  |  | 
10|`amount` | integer |  |  | 
11|`currency` | varchar |  |  | 
12|`code` | varchar |  |  | 
13|`ip` | varchar |  |  | 
14|`ip_country` | varchar |  |  | 
15|`created_at` | timestamp |  |  | 
16|`deleted_at` | timestamp |  |  | 
17|`total_tax` | integer |  |  | 
18|`updated_at` | timestamp |  |  | 
19|`discount` | boolean |  |  | 
