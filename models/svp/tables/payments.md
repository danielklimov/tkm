
payments
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | bigint | V |  | 
2|`amount` | money |  |  | 
3|`card_holder` | varchar |  |  | 
4|`expire_at` | timestamp |  |  | 
5|`failed` | boolean |  |  | 
6|`is_updated` | boolean |  |  | 
7|`ndc` | varchar |  |  | 
8|`payment_method` | varchar |  |  | 
9|`response` | jsonb |  |  | 
10|`transaction_date` | timestamp |  |  | 
11|`transaction_last_4_digits` | varchar |  |  | 
12|`transaction_payment_brand` | varchar |  |  | 
13|`transaction_status` | integer |  |  | 
14|`merchant_transaction_id` | varchar |  |  | 
15|`user_id` | bigint |  |  | 
16|`paid` | boolean |  |  | 
17|`created_at` | timestamp |  |  | 
18|`updated_at` | timestamp |  |  | 
19|`credits_count` | integer |  |  | 
20|`price_id` | bigint |  | [`prices`](prices.md) | 
