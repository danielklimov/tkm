
passport_recognitions
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | bigint | V |  | 
2|`country_id` | bigint |  | [`countries`](countries.md) | 
3|`nationality_id` | bigint |  | [`nationalities`](nationalities.md) | 
4|`recognizable_type` | varchar |  |  | 
5|`recognizable_id` | bigint |  |  | 
6|`recognized_data` | jsonb |  |  | 
7|`passport_mrz` | text |  |  | 
8|`data_match` | boolean |  |  | 
9|`image_hash` | varchar |  |  | 
10|`created_at` | timestamp |  |  | 
11|`updated_at` | timestamp |  |  | 
12|`submitted_data` | jsonb |  |  | 
