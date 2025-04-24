prometric_languages
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | uuid(language_code)
2|`language_code` | varchar |  |  | Two-letter language code
3|`name_ar` | varchar |  |  | Name in Arabic
4|`name_en` | varchar |  |  | Name in English
5|`is_active` | boolean |  |  | Available for selection
6|`created_at` | timestamp |  |  | 
7|`updated_at` | timestamp |  |  | 
8|`deleted_status` | varchar |  |  | ACTIVE, DELETED
