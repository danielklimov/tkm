
application_log
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | uuid | V |  | 
2|`type` | varchar |  |  | 
3|`user_id` | uuid |  | [`users`](users.md) | 
4|`description` | text |  |  | 
5|`data` | text |  |  | 
6|`context_id` | varchar |  |  | 
7|`created_at` | timestamp |  |  | 
