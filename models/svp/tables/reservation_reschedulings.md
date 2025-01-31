
reservation_reschedulings
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | bigint | V |  | 
2|`reservation_id` | bigint |  |  | 
3|`new_exam_session_id` | bigint |  | [`exam_sessions`](exam_sessions.md) | 
4|`old_exam_session_id` | bigint |  |  | 
5|`rescheduled_at` | timestamp |  |  | 
6|`created_at` | timestamp |  |  | 
7|`updated_at` | timestamp |  |  | 
