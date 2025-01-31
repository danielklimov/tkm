
temporary_seats
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | bigint | V |  | 
2|`expired_at` | timestamp |  |  | 
3|`exam_session_id` | bigint |  | [`exam_sessions`](exam_sessions.md) | 
4|`labor_id` | bigint |  | [`labors`](labors.md) | 
5|`created_at` | timestamp |  |  | 
6|`updated_at` | timestamp |  |  | 
