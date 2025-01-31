
admin_invite
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | uuid | V |  | 
2|`user_id` | uuid |  | [`users`](users.md) | 
3|`invited_user_id` | uuid |  | [`users`](users.md) | 
4|`token` | varchar |  |  | 
5|`email` | varchar |  |  | 
6|`invite_roles` | text |  |  | 
7|`created_at` | timestamp |  |  | 
8|`expire_at` | timestamp |  |  | 
9|`deleted_at` | timestamp |  |  | 
