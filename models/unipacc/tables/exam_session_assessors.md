exam_session_assessors
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | Autogenerated
2|`exam_session_id` | uuid |  | [`exam_sessions`](exam_sessions.md) | Exam session
3|`assessor_id` | uuid |  | [`assessors`](assessors.md) | Assessor that is attached to the exam session
4|`assessor_status` | varchar |  |  | Status of the assessor with this exam session. Enum values: PENDING CONFIRMED REJECTED ASSESSOR_WITHDRAWN
5|`created_at` | timestamp |  |  | 
6|`updated_at` | timestamp |  |  | 
7|`deleted_status` | varchar |  |  | ACTIVE, DELETED
