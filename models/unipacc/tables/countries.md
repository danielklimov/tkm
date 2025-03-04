countries
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION  | COMMENTS          
---|------|-----------|----|----|--------------|----------
1|`id` | uuid | V |  | Imitation of uuid created using ISO digital country code (during migration). Later on real random uuids may be used. | 
2|`name_en` | varchar |  |  | English name | 
3|`name_ar` | varchar |  |  | Arabic name | 
4|`nationality_name_en` | varchar |  |  | How a person that belongs to this nationality is caled, e.g. Kuwaiti, Peruvian etc. (English) | TODO: We are assuming that one country is linked to only one nationality. It has been designed like this in QVP and of course it is a generalization. If this generalization is enough for our purposes, we may leave it at that. Otherwise a separate table 'nationalities' is needed.
5|`nationality_name_ar` | varchar |  |  | Nationality name in arabic | 
6|`iso_3_code` | varchar |  |  | 3-letter ISO code | 
7|`iso_2_code` | varchar |  |  | 2-letter ISO code | 
8|`iso_no` | integer |  |  | ISO numeric country code | 
9|`svp_scenario` | varchar |  |  |  | a scenario used in svp flow for this country. One of: takamol_test_centers, prometric_test_centers, online verification.
10|`created_at` | timestamp |  |  |  | 
11|`updated_at` | timestamp |  |  |  | 
12|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record. | 
