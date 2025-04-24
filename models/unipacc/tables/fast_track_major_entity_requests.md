fast_track_major_entity_requests
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | autogen
2|`created_by_user_id` | uuid |  | [`users`](users.md) | 
3|`updated_by_user_id` | uuid |  | [`users`](users.md) | 
4|`entity_name_en` | varchar |  |  | Entity that submitted the request
5|`entity_name_ar` | varchar |  |  | Entity that submitted the request
6|`supplementary_document_ids` | text |  |  | TODO: strings encoded like this: a:1:{i:0;s:36:"627430b0-d398-4a7c-831e-f02a0ec532d7";}
7|`start_date` | timestamp |  |  | The fast track may have the dates when it becomes effective and when it expires
8|`end_date` | timestamp |  |  | The fast track may have the dates when it becomes effective and when it expires
9|`request_status` | varchar |  |  | one of: submitted, pending_updates, approved, rejected
10|`comment` | text |  |  | Free text
11|`major_entity_number` | varchar |  |  | I believe initially it was planned that there will be a separate table with major entities (4 entities exist rn), but seems it was not implemented. However, I'm thinking about keeping the standalone table for it  wit
12|`created_at` | timestamp |  |  | 
13|`updated_at` | timestamp |  |  | 
14|`deleted_status` | varchar |  |  | ACTIVE, DELETED
