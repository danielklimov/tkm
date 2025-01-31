
occupation
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | integer | V |  | Surrogate key
2|`occupation_category_id` | integer |  | [`occupation_category`](occupation_category.md) | 
3|`key` | integer |  |  | A key for sorting. TODO: how is it used?
4|`name_arabic` | varchar |  |  | 
5|`name_english` | varchar |  |  | 
6|`created_at` | timestamp |  |  | 
7|`updated_at` | timestamp |  |  | 
8|`deleted_at` | timestamp |  |  | 
9|`key_unique` | varchar |  |  | Another key for sorting. TODO: how is it used?
10|`name_arabic_unique` | varchar |  |  | TODO: how is it used?
11|`name_english_unique` | varchar |  |  | 
12|`description` | varchar |  |  | 
13|`main_tasks` | text |  |  | 
15|`any_major` | boolean |  |  | Signifies thet the occupation requires any major degree. TODO: is it correct?
16|`published` | boolean |  |  | The occupation will appear in web app. TODO: Correct?
17|`minimum_education_level_id` | integer |  | [`education_level`](education_level.md) | 
18|`updated_by_id` | uuid |  | [`users`](users.md) | 
19|`global` | boolean |  |  | 
20|`requirement_group` | integer |  |  | 
21|`subcategory_id` | uuid |  | [`occupation_subcategory`](occupation_subcategory.md) | 
