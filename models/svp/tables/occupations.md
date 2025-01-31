
occupations
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | bigint | V |  | surrogate key
2|`name` | varchar |  |  | Occupation name in English
3|`category_id` | bigint |  | [`categories`](categories.md) | 
4|`created_at` | timestamp |  |  | 
5|`updated_at` | timestamp |  |  | 
6|`occupation_key` | varchar |  |  | Numeric code. TODO: What is it used for?
7|`arabic_name` | varchar |  |  | Occupation name in Arabic
8|`qvp` | boolean |  |  | TODO: if true, does it mean this occupation belongs to qvp, rather than svp?
9|`active` | boolean |  |  | TODO: if false, what does it mean? Does it mean it is not visible in web app?
10|`mofa_mandated` | boolean |  |  | Skill verification for this occupation is mandated by MOFA (Ministry of Foreign Affairs). TODO: is it correct?
11|`lmh_mandated` | boolean |  |  | TODO: what is LMH?
