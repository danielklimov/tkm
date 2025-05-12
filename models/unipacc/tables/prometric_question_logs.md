prometric_question_logs
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | autoincrement
2|`name` | varchar |  |  | Exam name
3|`question_type` | varchar |  |  | Type of question. So far only one type was found - MultipleChoice.
4|`correct_answer` | varchar |  |  | Correct option(s), e.g.: A, D, DEF, 
5|`score_min` | integer |  |  | Minimum possible score - always 0
6|`score_max` | integer |  |  | Maximum score 1 or greater. E.g. if there are 3 correct answers, max score is 3
7|`category_name` | varchar |  |  | Always empty.
8|`created_at` | timestamp |  |  | 
9|`updated_at` | timestamp |  |  | 
10|`deleted_status` | varchar |  |  | ACTIVE, DELETED
