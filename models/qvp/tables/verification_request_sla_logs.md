
verification_request_sla_logs
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | integer | V |  | 
2|`request_id` | uuid |  | [`verification_request`](verification_request.md) | 
3|`user_id` | uuid |  | [`users`](users.md) | 
4|`timestamp_start` | varchar |  |  | 
5|`timestamp_stop` | varchar |  |  | 
6|`interval_seconds` | varchar |  |  | 
7|`status` | varchar |  |  | 
