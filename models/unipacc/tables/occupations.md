occupations
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | Auto-generated or manually assigned during migration
2|`name_en` | varchar |  |  | English name
3|`name_ar` | varchar |  |  | Arabic name
4|`code` | integer |  |  | Numeric code used for sorting
5|`occupation_category_id` | uuid |  | [`occupation_categories`](occupation_categories.md) | 
6|`occupation_subcategory_id` | uuid |  | [`occupation_subcategories`](occupation_subcategories.md) | 
7|`description` | varchar |  |  | Long description
8|`main_tasks` | text |  |  | Even longer description
9|`min_education_level_id` | uuid |  | [`education_levels`](education_levels.md) | 
10|`occupation_program_code` | varchar |  |  | One of: qvp, svp
11|`requirement_group` | integer |  |  | 0 - unassigned, 1 or 2. There are 2 requirement groups for QVP that define logic of calculation of eligibility score.
12|`is_global` | boolean |  |  | If true, the occupation must be verified for all nationalities (citizenships)
13|`is_any_major_degree` | boolean |  |  | true if any major degree can confirm this qualification
14|`is_published` | boolean |  |  | occupation is available in webapp
15|`is_mofa_mandated` | boolean |  |  | Qualification verification for this occupation is mandated by MOFA (Ministry of Foreign Affairs).
16|`is_lmh_mandated` | boolean |  |  | Skill verification for this occupation is mandated by LMH.
17|`created_at` | timestamp |  |  | 
18|`updated_at` | timestamp |  |  | 
19|`deleted_status` | varchar |  |  | ACTIVE, DELETED
