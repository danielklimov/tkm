
candidate
----------------------------

Info about job candidates.


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1 | `id` | integer | V | | 
2 | `user_id` | uuid |  | [`users`](users.md)| User ID used by candidate to log in.
3 | `second_name` | varchar |  | |
4 | `gender` | varchar |  | | Either 'Male', 'Female' or NULL
5 | `date_of_birth` | date |  | |
6 | `phone_number` | varchar |  | | Contact phone number without the country code.
7 | `country_code` | varchar |  | |
8 | `country` | varchar |  | | Candidate's current country of residence. TODO: or citizenship?
9 | `notification_language` | varchar |  |  | The language used for sending notifications. Not the user interface language.
10 | `alternate_name` | varchar |  | |
11 | `maiden_name` | varchar |  | |
12 | `former_married_name` | varchar |  | |
13 | `suffix` | varchar |  |  | Suffix used after name and surname, like Ph.D. or B.A. etc.
14 | `mothers_name` | varchar |  | |
15 | `deleted_at` | timestamp without time zone |  | | The record is not actually deleted, but is marked as deleted by setting this field to a non-null value.
16 | `passport_id` | uuid |  | [`passport`](passport.md)|
17 | `fast_track_immediate_record_id` | uuid |  | [`fast_track_immediate_record`](fast_track_immediate_record.md)|
