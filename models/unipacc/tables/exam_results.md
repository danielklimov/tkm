exam_results
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | Autoincr
2|`svp_booking_id` | uuid |  | [`svp_bookings`](svp_bookings.md) | A link with the booking for this exam
3|`original_cbt_score` | integer |  |  | CBT score as is, without corrections
4|`original_practical_score` | integer |  |  | Practical score as is, without corrections
5|`calculated_cbt_score` | integer |  |  | CNT exam score after corrections
6|`calculated_practical_score` | integer |  |  | Practical score after corrections
7|`response_id` | varchar |  |  | The "identity" value from The Prometric outcome response
8|`practical_response_id` | varchar |  |  | The "identity" value from The Prometric outcome response (practical exam)
9|`created_at` | timestamp |  |  | 
10|`updated_at` | timestamp |  |  | 
11|`deleted_status` | varchar |  |  | ACTIVE, DELETED
