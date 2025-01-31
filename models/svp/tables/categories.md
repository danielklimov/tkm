
categories
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | bigint | V |  | Surrogate key
2|`english_name` | varchar |  |  | 
3|`arabic_name` | varchar |  |  | 
4|`published` | boolean |  |  | TODO: Officialy available in web app?
5|`created_at` | timestamp |  |  | 
6|`updated_at` | timestamp |  |  | 
15|`exam_configuration` | jsonb |  |  | json that contains configuration parameters for an exam that can verify occupations belonging to this category
