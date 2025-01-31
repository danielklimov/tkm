
additional_payment_request
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | uuid | V |  | 
2|`verification_request_id` | uuid |  | [`verification_request`](verification_request.md) | 
3|`created_by_user_id` | uuid |  | [`users`](users.md) | 
4|`decided_by_user_id` | uuid |  | [`users`](users.md) | 
5|`status` | varchar |  |  | 
6|`created_at` | timestamp |  |  | 
7|`updated_at` | timestamp |  |  | 
8|`decided_at` | timestamp |  |  | 
9|`request_comment` | varchar |  |  | 
10|`file_id` | varchar |  |  | 
