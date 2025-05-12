countries
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | Imitation of uuid created using ISO 3-letter country code. Later on real random uuids may be used.
2|`name_en` | varchar |  |  | English name
3|`name_ar` | varchar |  |  | Arabic name
4|`nationality_name_en` | varchar |  |  | How a person that belongs to this nationality is caled, e.g. Kuwaiti, Peruvian etc. (English)
5|`nationality_name_ar` | varchar |  |  | Nationality name in arabic
6|`iso_3_code` | varchar |  |  | 3-letter ISO code
7|`iso_2_code` | varchar |  |  | 2-letter ISO code
8|`iso_no` | integer |  |  | ISO numeric country code
9|`svp_country_type` | varchar |  |  | One of: TARGETED, NON_TARGETED. TARGETED - exams are booked in Takamol test centers. NON_TARGETED - Prometric test centers are used.
10|`svp_test_type` | varchar |  |  | Exam type. On of: IN_PERSON, ONLINE. Nullable if svp_country_type = TARGETED
11|`is_mofa_qvp_mandated` | boolean |  |  | Qualification verification for citizens (residents?) or this country is mandated (required) by MOFA (Ministry of Foreign Affairs). See also: country_mofa_qvp_mandated_history
12|`is_mofa_svp_mandated` | boolean |  |  | Skill verification for citizens (residents?) or this country is mandated (required) by MOFA (Ministry of Foreign Affairs). See also: country_mofa_svp_mandated_history
13|`is_lmh_qvp_mandated` | boolean |  |  | Qualification verification for this country is mandated by LMH.
14|`is_lmh_svp_mandated` | boolean |  |  | Skill verification for this country is mandated by LMH.
15|`svp_certificate_price` | numeric(18,2) |  |  | Price (in USD) for an svp test in this country.
16|`created_at` | timestamp |  |  | 
17|`updated_at` | timestamp |  |  | 
18|`deleted_status` | varchar |  |  | ACTIVE, DELETED
