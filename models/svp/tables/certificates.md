
certificates
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | bigint | V |  | 
2|`labor_id` | bigint |  | [`labors`](labors.md) | 
3|`country_id` | bigint |  | [`countries`](countries.md) | 
4|`category_id` | bigint |  | [`categories`](categories.md) | 
5|`payment_id` | bigint |  | [`payments`](payments.md) | 
6|`certificate_number` | varchar |  |  | 
7|`valid_until` | timestamp |  |  | 
8|`created_at` | timestamp |  |  | 
9|`updated_at` | timestamp |  |  | 
10|`withdrawal_id` | bigint |  | [`withdrawals`](withdrawals.md) | 
11|`free` | boolean |  |  | 
12|`sended_certificates_count` | integer |  |  | 
14|`access_token` | varchar |  |  | 
