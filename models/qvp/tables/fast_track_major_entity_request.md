
fast_track_major_entity_request
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | uuid | V |  | 
2|`created_by_id` | uuid |  | [`users`](users.md) | 
3|`updated_by_id` | uuid |  | [`users`](users.md) | 
4|`entity_name_english` | varchar |  |  | 
5|`entity_name_arabic` | varchar |  |  | 
6|`supplementary_document_ids` | text |  |  | 
7|`start_date` | timestamp |  |  | 
8|`end_date` | timestamp |  |  | 
9|`created_at` | timestamp |  |  | 
10|`updated_at` | timestamp |  |  | 
11|`status` | varchar |  |  | 
12|`comment` | text |  |  | 
13|`major_entity_number` | varchar |  |  | 
