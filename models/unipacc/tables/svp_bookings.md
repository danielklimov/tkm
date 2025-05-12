svp_bookings
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | Autoincr
2|`exam_result` | varchar |  |  | One of: PENDING, PASSED, FAILED
3|`cbt_exam_status` | varchar |  |  | One of: RESERVED, PENDING, COMPLETED, CANCELED, WITHDRAWN, PAYMENT_FAILED
4|`certificate_id` | uuid |  | [`svp_certificates`](svp_certificates.md) | Skill verification certificate, issued as a result of passing the exam
5|`applicant_id` | uuid |  | [`applicants`](applicants.md) | Applicant that booked an exam session
6|`exam_session_id` | uuid |  | [`exam_sessions`](exam_sessions.md) | An exam session that was booked
7|`payment_id` | uuid |  | [`payments`](payments.md) | TODO: Payment for the exam. Payments for qvp and svp should be united into one table. It's not yet ready
8|`cancellation_reason` | varchar |  |  | Description why the booking was cancelled. Free text, not an enum.
9|`is_paid` | boolean |  |  | A flag showing that the booking is paid either with credits or with a card payment
10|`keycode` | varchar |  |  | Prometric code
11|`cbt_eligibility_status` | varchar |  |  | When the exam is started, we send the Create Eligibility Request to Prometric, and Prometric returns -1 (failed) or 1 (success) as the response which we store in this column
12|`practical_eligibility_status` | varchar |  |  | When the exam is started, we send the Create Eligibility Request to Prometric, and Prometric returns -1 (failed) or 1 (success) as the response which we store in this column
13|`occupation_id` | uuid |  | [`occupations`](occupations.md) | The occupation that is going to be verified
14|`edit_reason` | varchar |  |  | Admins can update the bookings, if they update - the comment is required and stored in this field
15|`is_hidden` | boolean |  |  | When the reservation is created - it is by default is_hidden: true till payment is made Once User successfully made the payment - change to is_hidden: false In the System only is_hidden: false are shown
16|`practical_exam_status` | integer |  |  | One of: RESERVED, PENDING, COMPLETED, CANCELED, WITHDRAWN, PAYMENT_FAILED
17|`access_token` | varchar |  |  | Access token is a part of Reservation Ticket URL to attend the exam (randomly generated)
18|`cancelled_by_user_id` | uuid |  | [`users`](users.md) | The user that cancelled the booking
19|`cbt_started_at` | timestamp |  |  | 
20|`cbt_result_received_at` | timestamp |  |  | 
21|`practical_started_at` | timestamp |  |  | 
22|`practical_result_received_at` | timestamp |  |  | 
23|`cbt_prometric_outcome_response` | text |  |  | json
24|`practical_prometric_outcome_response` | text |  |  | json
25|`prometric_data` | text |  |  | json.Prometric data (or metadata) about exam
26|`created_at` | timestamp |  |  | 
27|`updated_at` | timestamp |  |  | 
28|`deleted_status` | varchar |  |  | ACTIVE, DELETED
