professional_certificates
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | 
2|`name_en` | varchar |  |  | certificate name in English
3|`name_ar` | varchar |  |  | certificate name in Arabic
4|`institute_name_en` | varchar |  |  | Institute or organization that issues the certificate
5|`institute_name_ar` | varchar |  |  | Institute or organization that issues the certificate
6|`is_online_version` | boolean |  |  | Possible to check the certificate online
7|`online_version_url` | varchar |  |  | URL that points to certification institute website
8|`is_published` | boolean |  |  | shown in webapp
9|`updated_by` | uuid |  | [`users`](users.md) | 
10|`updated_at` | timestamp |  |  | 
11|`deleted_at` | timestamp |  |  | 
12|`created_at` | timestamp |  |  | 
13|`updated_at` | timestamp |  |  | 
14|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record.
