phone_country_codes
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | Initially a copy of actual country phone code, but not guaranteed to always coincide with it. Other codes may be used in special cases.
2|`phone_code` | varchar |  |  | Phone code or "dial-in code"
3|`country_id` | uuid |  | [`countries`](countries.md) | The country (or primary country) that this code currently belongs to. null if not applicable
4|`descr` | varchar |  |  | Optional comments
5|`created_at` | timestamp |  |  | 
6|`updated_at` | timestamp |  |  | 
7|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record.
