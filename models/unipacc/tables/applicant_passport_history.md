applicant_passport_history
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | Surrogate key
2|`applicant_id` | uuid |  | [`applicants`](applicants.md) | Applicant - the owner of the passport
3|`passport_id` | uuid |  | [`passports`](passports.md) | The cuurrently active passport
4|`valid_from` | date |  |  | The date when this record becomes active
5|`created_at` | timestamp |  |  | System field - date and time when the record was created
6|`updated_at` | timestamp |  |  | System field - date and time when the record was modified (or created when the record is new)
7|`deleted_status` | varchar |  |  | ACTIVE, DELETED
