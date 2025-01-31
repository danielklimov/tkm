
verification_request_sla_holds
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | uuid | V |  | 
3|`user_id` | uuid |  | [`users`](users.md) | 
4|`reason` | varchar |  |  | 
5|`description` | text |  |  | 
6|`revoke_comment` | varchar |  |  | 
7|`sla_log_id` | integer |  | [`verification_request_sla_logs`](verification_request_sla_logs.md) | 
8|`previous_status` | varchar |  |  | 
