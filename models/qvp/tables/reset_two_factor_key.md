
reset_two_factor_key
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | integer | V |  | 
2|`user_id` | uuid |  | [`users`](users.md) | 
3|`token` | varchar |  |  | 
4|`used` | boolean |  |  | 
5|`expire_at` | timestamp |  |  | 
6|`deleted_at` | timestamp |  |  | 
