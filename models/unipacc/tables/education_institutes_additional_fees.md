education_institutes_additional_fees
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION  | COMMENTS          
---|------|-----------|----|----|--------------|----------
1|`id` | uuid | V |  | 
2|`education_institute_id` | uuid |  | [`education_institutes`](education_institutes.md) | 
3|`education_level_id` | uuid |  | [`education_levels`](education_levels.md) | 
4|`major_id` | integer |  | [`majors`](majors.md) | 
5|`updated_by_user_id` | uuid |  | [`users`](users.md) | 
6|`fee_amount` | integer |  |  | Fee amount in USD
7|`is_published` | boolean |  |  | Show this record in web interface and use it in business logic
8|`ministry_id` | varchar |  |  | An id in xls file from the Ministry
9|`created_at` | timestamp |  |  | 
10|`updated_at` | timestamp |  |  | 
11|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record.
