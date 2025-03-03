
applicant_passport_history
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION  | COMMENTS          
---|------|-----------|----|----|--------------|----------
1|`applicant_id` | uuid | V | [`applicants`](applicants.md) | Applicant - the owner of the passport | 
2|`passport_id` | uuid | V | [`passports`](passports.md) | The cuurrently active passport | 
3|`valid_from` | date | V |  | The date when this record becomes active | 
4|`created_at` | timestamp |  |  | System field - date and time when the record was created | 
5|`updated_at` | timestamp |  |  | System field - date and time when the record was modified (or created when the record is new) | 
6|`deleted_status` | integer | V |  | 0 - active record, 1 - deleted record. | 
