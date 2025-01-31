
passport
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | uuid | V |  | 
2|`user_id` | varchar |  |  | 
3|`nationality_name` | varchar |  |  | 
4|`number` | varchar |  |  | 
5|`expiration_date` | date |  |  | 
6|`deleted_at` | timestamp |  |  | 
7|`nationality_id` | uuid |  | [`verification_request_nationality`](verification_request_nationality.md) | 
