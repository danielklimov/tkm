
verification_request_sla_holds
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | uuid | V |  | 
3|`user_id` | uuid |  | [`users`](users.md) | 
4|`reason` | varchar |  |  | 
5|`description` | varchar |  |  | 
6|`revoke_comment` | varchar |  |  | 
7|`sla_log_id` | integer |  |  | 
8|`previous_status` | varchar |  |  | 
