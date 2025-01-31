
exam_session_assessors
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | bigint | V |  | 
2|`exam_session_id` | bigint |  | [`exam_sessions`](exam_sessions.md) | 
3|`assessor_id` | bigint |  | [`assessors`](assessors.md) | 
4|`status` | integer |  |  | 
5|`created_at` | timestamp |  |  | 
6|`updated_at` | timestamp |  |  | 
