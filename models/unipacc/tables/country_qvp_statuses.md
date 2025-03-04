country_qvp_statuses
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`country_id` | integer | V | [`country`](country.md) | 
2|`mandated_from_date` | date |  |  | Date starting at which the requirement for verification is set for this country_id. If the requirement is lifted later, the record should be marked as record_status = 1 meaning it is marked as deleted.
3|`created_at` | timestamp |  |  | 
4|`updated_at` | timestamp |  |  | 
5|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record.
