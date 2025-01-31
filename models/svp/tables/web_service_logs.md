
web_service_logs
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | bigint | V |  | 
2|`base_url` | varchar |  |  | 
3|`path` | varchar |  |  | 
4|`body` | jsonb |  |  | 
5|`response` | jsonb |  |  | 
6|`response_code` | integer |  |  | 
7|`created_at` | timestamp |  |  | 
8|`updated_at` | timestamp |  |  | 
9|`country_id` | bigint |  | [`countries`](countries.md) | 
