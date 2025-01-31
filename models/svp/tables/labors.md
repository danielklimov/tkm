
labors
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | bigint | V |  | 
2|`national_id` | varchar |  |  | National ID document/card number
3|`full_name` | varchar |  |  | Name Surname in English
4|`passport_number` | varchar |  |  | Passport number
5|`occupation_id` | bigint |  |  | TODO: only nulls found. Not used?
6|`legislator_id` | bigint |  |  | TODO: nulls. Not used?
7|`created_at` | timestamp |  |  | 
8|`updated_at` | timestamp |  |  | 
9|`group_id` | bigint |  | [`groups`](groups.md) | Deprecated flow
10|`test_center_id` | bigint |  | [`test_centers`](test_centers.md) | Test center ID selected by user for taking an exam
11|`category_id` | bigint |  | [`categories`](categories.md) | Category of occupation. TODO: Is it used? Occupation_id is null?
12|`country_id` | bigint |  | [`countries`](countries.md) | Labor's country of residence
13|`user_id` | bigint |  | [`users`](users.md) | Reference to a user account associated with this labor
14|`withdrawal_id` | bigint |  | [`withdrawals`](withdrawals.md) | 
15|`full_name_ar` | varchar |  |  | Full name in Arabic
16|`exam_score` | integer |  |  | TODO: Deprecated?
17|`exam_result` | integer |  |  | TODO: Deprecated?
18|`exam_date` | date |  |  | TODO: Deprecated?
19|`email` | varchar |  |  | 
20|`registered` | boolean |  |  | TODO: registered for an exam?
21|`nationality_id` | integer |  |  | TODO: It is a reference to a list of countries. Does it mean citizenship, or ethnic group which the labor associates himself with?
22|`date_of_birth` | date |  |  | 
23|`passport_expiration_date` | date |  |  | 
24|`sex` | integer |  |  | 0 - male, 1 - female or nulls
25|`education_level` | varchar |  |  | One of: unlearned, middle, learned, primary, secondary, diploma TODO: is there any more?
26|`knowledge_level` | varchar |  |  | One or several values from this list: certificated, experienced, erudite. If several - delimited by comma TODO: is there more values?
27|`experience_level` | varchar |  |  | One of: less_than_3, between_3_and_5, greater_than_5 (years?)
28|`institute_name` | varchar |  |  | Institute or government agency that issued occupation certificate in case when knowledge_level includes 'certificated'
