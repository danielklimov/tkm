fast_track_major_entity_request_docs
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | autogen
2|`fast_track_major_entity_request_id` |  |  | [`fast_track_major_entity_requests`](fast_track_major_entity_requests.md) | 
3|`supplementary_document_id` | uuid |  | [`file_storage`](file_storage.md) | 
4|`seq_number` | integer |  |  | Sequential number of this attached document within one fast_track_immediate_request
5|`created_at` | timestamp |  |  | 
6|`updated_at` | timestamp |  |  | 
7|`deleted_status` | varchar |  |  | ACTIVE, DELETED
