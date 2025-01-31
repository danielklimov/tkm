
prometric_exam_result_logs
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | bigint | V |  | 
2|`prometric_exam_log_id` | bigint |  | [`prometric_exam_logs`](prometric_exam_logs.md) | 
3|`exam_session_id` | bigint |  | [`exam_sessions`](exam_sessions.md) | 
4|`reservation_id` | bigint |  | [`reservations`](reservations.md) | 
5|`start_datetime` | timestamp |  |  | 
6|`end_datetime` | timestamp |  |  | 
7|`duration` | integer |  |  | 
8|`restarts_count` | integer |  |  | 
9|`correct_questions_count` | integer |  |  | 
10|`incorrect_questions_count` | integer |  |  | 
11|`skipped_questions_count` | integer |  |  | 
12|`score_value` | integer |  |  | 
13|`score_percent` | double precision |  |  | 
14|`pass_indicator` | varchar |  |  | 
15|`grade` | varchar |  |  | 
16|`created_at` | timestamp |  |  | 
