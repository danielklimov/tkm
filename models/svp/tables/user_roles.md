
user_roles
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | bigint | V |  | 
2|`user_id` | bigint |  | [`users`](users.md) | 
3|`role_id` | bigint |  | [`roles`](roles.md) | 
4|`created_at` | timestamp |  |  | 
5|`updated_at` | timestamp |  |  | 
