
prometric_answer_logs
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | bigint | V |  | 
2|`prometric_question_log_id` | bigint |  | [`prometric_question_logs`](prometric_question_logs.md) | 
3|`prometric_exam_result_log_id` | bigint |  | [`prometric_exam_result_logs`](prometric_exam_result_logs.md) | 
4|`sequence` | integer |  |  | 
5|`duration` | integer |  |  | 
6|`weight` | integer |  |  | 
7|`user_answer` | varchar |  |  | 
8|`score` | integer |  |  | 
9|`scored` | boolean |  |  | 
10|`presented` | boolean |  |  | 
11|`created_at` | timestamp |  |  | 
