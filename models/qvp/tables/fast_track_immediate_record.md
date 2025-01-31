
fast_track_immediate_record
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | uuid | V |  | 
3|`passport_number` | varchar |  |  | Passport number of the candidate for whom this fast track record was created.
4|`entity_name_english` | varchar |  |  | Entity - means organization (company) that requires fast track
5|`entity_name_arabic` | varchar |  |  | 
6|`created_at` | timestamp |  |  | 
7|`updated_at` | timestamp |  |  | 
"8|`status` | varchar |  |  | fast track status. TODO; find out what other values except 'active' there can be"
9|`nationality_id` | uuid |  | [`verification_request_nationality`](verification_request_nationality.md) | Nationality of the user that this fast track record is created for
