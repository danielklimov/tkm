
test_center_status_requests
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | bigint | V |  | 
2|`test_center_id` | bigint |  | [`test_centers`](test_centers.md) | 
3|`user_id` | bigint |  |  | 
4|`expires_at` | timestamp |  |  | 
5|`status` | integer |  |  | 
6|`test_center_status` | integer |  |  | 
7|`created_at` | timestamp |  |  | 
8|`updated_at` | timestamp |  |  | 
