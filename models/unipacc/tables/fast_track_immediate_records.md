fast_track_immediate_records
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION  | COMMENTS          
---|------|-----------|----|----|--------------|----------
1|`passport_number` | varchar |  |  | Passport number of the candidate for whom this fast track record was created. | 
2|`entity_name_english` | varchar |  |  | Entity - means organization (company) that requires fast track | 
3|`entity_name_arabic` | varchar |  |  |  | 
4|`created_at` | timestamp |  |  |  | 
5|`updated_at` | timestamp |  |  |  | 
6|`status` | varchar |  |  | fast track status. TODO; find out what other values except 'active' there can be | 
7|`country_id` | integer |  | [`countries`](countries.md) | Country of citizenship of the user that this fast track record is created for | 
8|`created_at` | timestamp |  |  |  | 
9|`updated_at` | timestamp |  |  |  | 
10|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record. | 
