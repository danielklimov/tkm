
permissions
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | bigint | V |  | 
2|`permission_name` | varchar |  |  | 
3|`permission_group` | varchar |  |  | 
4|`country_id` | bigint |  | [`countries`](countries.md) | 
5|`role_id` | bigint |  | [`roles`](roles.md) | 
