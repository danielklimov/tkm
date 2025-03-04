occupation_categories
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION  | COMMENTS          
---|------|-----------|----|----|--------------|----------
1|`id` | uuid | V |  | Auto-generated or manually assigned during migration | 
2|`name_en` | varchar |  |  | Name in English | 
3|`name_ar` | varchar |  |  | Name in Arabic | 
4|`code` | varchar |  |  | User-defined numeric code used for sorting | 
5|`verification_type_code` | integer |  |  | 1 - qualification, 2 - skills | 
6|`min_years_of_experience` | integer |  |  | Minimum years of experience required for verification for any occupation under this category | 
7|`is_published` | boolean |  |  | Officialy available in web app | 
8|`svp_exam_conf` | jsonb |  |  | Exam configuration params. In use only by SVP | 
9|`created_at` | timestamp |  |  |  | 
10|`updated_at` | timestamp |  |  |  | 
11|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record. | 
