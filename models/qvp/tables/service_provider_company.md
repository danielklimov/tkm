
service_provider_company
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | uuid | V |  | 
2|`bank_account` | uuid |  | [`bank_account`](bank_account.md) | 
4|`name_english` | varchar |  |  | 
5|`company_country` | varchar |  |  | 
6|`establishment_number` | varchar |  |  | 
8|`created_at` | timestamp |  |  | 
9|`updated_at` | timestamp |  |  | 
10|`last_verification_request_assign_date` | timestamp |  |  | 
11|`deleted_at` | timestamp |  |  | 
12|`is_ready` | boolean |  |  | 
15|`name_arabic` | varchar |  |  | 
16|`license_number` | varchar |  |  | 
17|`name_registered` | varchar |  |  | 
18|`license_issuing_date` | date |  |  | 
19|`license_end_date` | date |  |  | 
20|`email` | varchar |  |  | 
21|`phone_number` | varchar |  |  | 
22|`website` | varchar |  |  | 
23|`building_number` | varchar |  |  | 
24|`street_name` | varchar |  |  | 
25|`neighborhood` | varchar |  |  | 
26|`city` | varchar |  |  | 
27|`postal_code` | varchar |  |  | 
28|`additional_number` | varchar |  |  | 
30|`bank_account_holder_name` | varchar |  |  | 
31|`bank_account_confirmation_file` | uuid |  | [`file_storage`](file_storage.md) | 
32|`phone_number_prefix` | varchar |  |  | 
33|`phone_number_country_code` | varchar |  |  | 
34|`is_filled` | boolean |  |  | 
35|`agreed_on_terms_and_conditions` | boolean |  |  | 
36|`location_data` | text |  |  | 
37|`license_document_file_id` | varchar |  |  | 
38|`status` | varchar |  |  | 
39|`verification_types` | json |  |  | 
40|`internal` | boolean |  |  | 
