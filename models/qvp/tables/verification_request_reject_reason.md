
verification_request_reject_reason
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | integer | V |  | 
2|`reason_id` | integer |  | [`reject_reason`](reject_reason.md) | 
3|`request_id` | uuid |  | [`verification_request`](verification_request.md) | 
4|`comment` | text |  |  | 
5|`created_at` | timestamp |  |  | 
