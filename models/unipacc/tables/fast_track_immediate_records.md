fast_track_immediate_records
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | 
2|`passport_number` | varchar |  |  | Passport number of the candidate for whom this fast track record was created.
3|`entity_name_en` | varchar |  |  | Entity - means organization (company) that requires fast track process
4|`entity_name_ar` | varchar |  |  | 
5|`fast_track_status` | varchar |  |  | fast track status. TODO; find out what other values except 'active' there can be
6|`country_id` | uuid |  | [`countries`](countries.md) | Country of citizenship of the user that this fast track record is created for
7|`created_at` | timestamp |  |  | 
8|`updated_at` | timestamp |  |  | 
9|`deleted_status` | varchar |  |  | ACTIVE, DELETED
