
prometric_codes
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | bigint | V |  | 
2|`language_code` | varchar |  |  | 
3|`code` | varchar |  |  | 
4|`category_id` | bigint |  | [`categories`](categories.md) | 
5|`created_at` | timestamp |  |  | 
6|`updated_at` | timestamp |  |  | 
7|`non_targeted` | boolean |  |  | 
