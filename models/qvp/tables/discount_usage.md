
discount_usage
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | integer | V |  | 
2|`discount_id` | integer |  | [`discount`](discount.md) | 
3|`verification_request_id` | uuid |  | [`verification_request`](verification_request.md) | 
4|`uuid` | uuid |  |  | 
5|`user_id` | uuid |  |  | 
6|`passport_number` | varchar |  |  | 
7|`created_at` | timestamp |  |  | 
