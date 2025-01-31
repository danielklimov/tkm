
candidate
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | integer | V |  | 
2|`user_id` | uuid |  | [`users`](users.md) | User ID used by candidate to log in.
3|`second_name` | varchar |  |  | Users second name (same as middle name) if he has any
4|`gender` | varchar |  |  | Gender. Can be 'Male', 'Female' or NULL
5|`date_of_birth` | date |  |  | 
6|`phone_number` | varchar |  |  | Contact phone number without the country code.
7|`country_code` | varchar |  |  | Telephone country code
9|`country` | varchar |  |  | Candidate's current country of residence. TODO: or citizenship?
10|`notification_language` | varchar |  |  | A language used for sending notifications. Not the user interface language. two-letter code - en, ar of null
13|`alternate_name` | varchar |  |  | TODO: is there an example of how this field is actually used? What does it mean?
14|`maiden_name` | varchar |  |  | 
15|`former_married_name` | varchar |  |  | 
16|`suffix` | varchar |  |  | Suffix used after name and surname, like Ph.D. or B.A. etc.
17|`mothers_name` | varchar |  |  | 
18|`deleted_at` | timestamp |  |  | The record is not actually deleted, but is marked as deleted by setting this field to a non-null value.
19|`passport_id` | uuid |  | [`passport`](passport.md) | 
20|`fast_track_immediate_record_id` | uuid |  | [`fast_track_immediate_record`](fast_track_immediate_record.md) | If assigned, a reference to a fast track record
