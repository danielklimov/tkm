assessors
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | Auto-generated or manually generated during migration
2|`date_of_birth` | date |  |  | 
3|`gender` | varchar |  |  | Male, Female or equivalents in Arabic, or nulls
4|`institute_name` | varchar |  |  | TODO: An assessor is connected with an institute (organization) in some way. Does he work in that institute as an employee? Is he certified by that institute in some way?
5|`passport_id` | uuid |  | [`passports`](passports.md) | Currently active passport
6|`national_id` | varchar |  |  | national id card/document number
7|`it_skills` | varchar |  |  | Information technology skills. Enum.
8|`international_experience` | varchar |  |  | International experience (years). Enum.
9|`experience` | varchar |  |  | Experience in (years) - enumeration: 
10|`is_certified_assessor` | boolean |  |  | Assessors could be certified by some 3rd parties: schools, institutes, course, universitites, etc. (outside of Takamol), if during the registration assessor marks 'certified_assessor' checkbox,
then the assessor must upload the experience_certificate 
11|`is_online_tools_skills` | boolean |  |  | Does the assessor have skillts for online tools: Skype, MS Office, etc.
12|`is_professional_qualification` | boolean |  |  | Does the assessor have the professional qualification for occupations that he assesses.
13|`location_country_id` | uuid |  | [`countries`](countries.md) | The country that assessor is located in
14|`user_id` | uuid |  | [`users`](users.md) | User account used by this assessor to log in.
15|`nationality_id` | uuid |  | [`countries`](countries.md) | Nationality (citizenship) of the assessor
16|`registration_method` | varchar |  |  | Self-registered or invited by Takamol. Enum.
17|`review_state` | varchar |  |  | Assessor's current state of being able to conduct assessments. Enumeration.
18|`test_center_id` | uuid |  | [`test_centers`](test_centers.md) | Test center the assessor is working from
19|`rejection_reason` | text |  |  | Reason why the assessor was rejected
20|`document_type` | varchar |  |  | TODO: Type of document that identifies the assessor. In stg v2 it's always 'passport'. As we already have passports table there is no need to store this field here
21|`international_qualifications` | varchar |  |  | TODO: One or more of: no_international_qualification, degree, diploma, training. Move to a separate table.
22|`full_name` | varchar |  |  | Assessor's full name.
23|`created_at` | timestamp |  |  | 
24|`updated_at` | timestamp |  |  | 
25|`deleted_status` | varchar |  |  | ACTIVE, DELETED
