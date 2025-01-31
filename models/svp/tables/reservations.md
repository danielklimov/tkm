
reservations
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | bigint | V |  | 
2|`exam_result` | integer |  |  | 
4|`cbt_exam_status` | integer |  |  | 
5|`certificate_id` | bigint |  | [`certificates`](certificates.md) | 
6|`labor_id` | bigint |  | [`labors`](labors.md) | 
7|`exam_session_id` | bigint |  | [`exam_sessions`](exam_sessions.md) | 
8|`created_at` | timestamp |  |  | 
9|`updated_at` | timestamp |  |  | 
10|`payment_id` | bigint |  | [`payments`](payments.md) | 
11|`cancellation_reason` | varchar |  |  | 
12|`paid` | boolean |  |  | 
13|`start_exam_url` | varchar |  |  | 
14|`keycode` | varchar |  |  | 
15|`cbt_eligibility_status` | varchar |  |  | 
16|`practical_eligibility_status` | varchar |  |  | 
17|`occupation_id` | bigint |  | [`occupations`](occupations.md) | 
18|`edit_reason` | varchar |  |  | 
19|`hidden` | boolean |  |  | 
20|`practical_exam_status` | integer |  |  | 
21|`access_token` | varchar |  |  | 
22|`cancelled_by_user_id` | bigint |  | [`users`](users.md) | 
23|`exam_error` | varchar |  |  | 
24|`cbt_started_at` | timestamp |  |  | 
25|`cbt_result_received_at` | timestamp |  |  | 
26|`practical_started_at` | timestamp |  |  | 
27|`practical_result_received_at` | timestamp |  |  | 
28|`cbt_prometric_outcome_response` | jsonb |  |  | 
29|`practical_prometric_outcome_response` | jsonb |  |  | 
30|`initially_completed_at` | timestamp |  |  | 
