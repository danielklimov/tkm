
assessors
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | bigint | V |  | Surrogate key.
2|`date_of_birth` | date |  |  | 
3|`gender` | varchar |  |  | Male, Female or equivalents in Arabic, or nulls
4|`cities` | ARRAY |  |  | Array of cities that the assessor is servicing. TODO: correct?
5|`institute_name` | varchar |  |  | TODO: An assessor is connected with an institute (organization) in some way. Does he work in that institute as an employee? Is he certified by that institute in some way?
6|`passport_number` | varchar |  |  | passport number
7|`national_id` | varchar |  |  | national id card/document number
8|`languages` | ARRAY |  |  | languages spoken by the assessor as an array of two-letter codes
9|`it_skills` | integer |  |  | 0,1 or 2. TODO: Information technology skills? Grade (score) 0 to 2
11|`international_experience` | integer |  |  | Grades 0 to 2
12|`educational_qualification` | integer |  |  | Grades 0 to 2
13|`experience` | integer |  |  | Grades 0 to 9.
14|`certified_assessor` | boolean |  |  | TODO: certified by institute_name ?
15|`online_tools_skills` | boolean |  |  | 
16|`professional_qualification` | boolean |  |  | 
17|`country_id` | bigint |  |  | The country that assessor is located in
18|`user_id` | bigint |  |  | user used for login
20|`nationality_id` | bigint |  |  | citizenship of the assessor TODO: check
21|`created_at` | timestamp |  |  | 
22|`updated_at` | timestamp |  |  | 
24|`registration_method` | integer |  |  | TODO: what is it? Values found: 0 and 1
25|`review_state` | integer |  |  | TODO: what is it? Numbers 0 to 6
26|`test_center_id` | bigint |  | [`test_centers`](test_centers.md) | Test center the assessor is working from
27|`rejection_reason` | text |  |  | Reason why the assessor was rejected
28|`document_type` | varchar |  |  | Document that identifies the assessor. Values found: 'passport' or null
29|`document_expiration_date` | date |  |  | Expiration date of identifying document which number is stored in `passport_number` field and type is stored in `document_type' field. TODO: check.
30|`international_qualifications` | varchar |  |  | One or more of: no_international_qualification, degree, diploma, training. Separated by colons 
31|`full_name` | varchar |  |  | Assessor's full name.
