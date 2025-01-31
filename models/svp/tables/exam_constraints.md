
exam_constraints
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | bigint | V |  | 
2|`reservation_rescheduling` | integer |  |  | 
3|`reservation_duration` | integer |  |  | 
4|`payment_processing_msg_duration` | integer |  |  | 
5|`working_hours` | integer |  |  | 
6|`start_time` | varchar |  |  | 
7|`created_at` | timestamp |  |  | 
8|`updated_at` | timestamp |  |  | 
9|`session_min_hours_before_start` | integer |  |  | 
10|`admin_reservation_cancellation_time_limit` | integer |  |  | 
11|`admin_session_cancellation_time_limit` | integer |  |  | 
12|`test_center_owner_reservation_cancellation_time_limit` | integer |  |  | 
13|`test_center_owner_session_cancellation_time_limit` | integer |  |  | 
14|`labor_reservation_cancellation_time_limit` | integer |  |  | 
15|`reschedule_allowed_time` | integer |  |  | 
16|`start_exam_session_allowed_time` | integer |  |  | 
17|`settings` | jsonb |  |  | 
