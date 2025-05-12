svp_exam_session_temp_seats
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | autoincrement
2|`expired_at` | timestamp |  |  | The expiration time of temporarily seats (the temporarilly seat is created for 20 minutes allowing user to make a payment for a reservation)
3|`exam_session_id` | uuid |  | [`exam_sessions`](exam_sessions.md) | Exam session where the reservation is going to be made
4|`applicant_id` | uuid |  | [`applicants`](applicants.md) | Labor who is creating a reservation.
5|`created_at` | timestamp |  |  | 
5|`created_at` | timestamp |  |  | 
6|`updated_at` | timestamp |  |  | 
6|`updated_at` | timestamp |  |  | 
7|`deleted_status` | varchar |  |  | ACTIVE, DELETED
7|`deleted_status` | varchar |  |  | ACTIVE, DELETED
