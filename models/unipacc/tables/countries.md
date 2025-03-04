countries
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | Imitation of uuid created using ISO digital country code (during migration). Later on real random uuids may be used.
2|`name_en` | varchar |  |  | English name
3|`name_ar` | varchar |  |  | Arabic name
4|`nationality_name_en` | varchar |  |  | How a person that belongs to this nationality is caled, e.g. Kuwaiti, Peruvian etc. (English)
5|`nationality_name_ar` | varchar |  |  | Nationality name in arabic
6|`iso_3_code` | varchar |  |  | 3-letter ISO code
7|`iso_2_code` | varchar |  |  | 2-letter ISO code
8|`iso_no` | integer |  |  | ISO numeric country code
9|`svp_country_type` | varchar |  |  | A way we define what verification flow is used for a specific country. One of: targeted, non_targeted
10|`is_mofa_mandated` | boolean |  |  | Qualification and skill verification for citizens (residents?) or this country is mandated (required) by MOFA (Ministry of Foreign Affairs).
11|`created_at` | timestamp |  |  | 
12|`updated_at` | timestamp |  |  | 
13|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record.
