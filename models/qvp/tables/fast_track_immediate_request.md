
fast_track_immediate_request
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | uuid | V |  | 
2|`nationality_id` | uuid |  | [`verification_request_nationality`](verification_request_nationality.md) | 
3|`created_by_id` | uuid |  | [`users`](users.md) | 
4|`updated_by_id` | uuid |  | [`users`](users.md) | 
5|`passport_number` | varchar |  |  | 
6|`entity_name_english` | varchar |  |  | 
7|`entity_name_arabic` | varchar |  |  | 
8|`supplementary_document_ids` | text |  |  | 
9|`created_at` | timestamp |  |  | 
10|`updated_at` | timestamp |  |  | 
11|`status` | varchar |  |  | 
12|`comment` | text |  |  | 
