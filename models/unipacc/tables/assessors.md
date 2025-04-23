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
7|`languages` | ARRAY |  |  | languages spoken by the assessor as an array of two-letter codes
8|`it_skills` | varchar |  |  | Information technology skills. Enum.
9|`international_experience` | varchar |  |  | International experience (years). Enum.
10|`experience` | varchar |  |  | Experience in (years) - enumeration: 
11|`is_certified_assessor` | boolean |  |  | Assessors could be certified by some 3rd parties: schools, institutes, course, universitites, etc. (outside of Takamol), if during the registration assessor marks 'certified_assessor' checkbox,
then the assessor must upload the experience_certificate 
12|`is_online_tools_skills` | boolean |  |  | Does the assessor have skillts for online tools: Skype, MS Office, etc.
13|`is_professional_qualification` | boolean |  |  | Does the assessor have the professional qualification for occupations that he assesses.
14|`location_country_id` | uuid |  | [`countries`](countries.md) | The country that assessor is located in
15|`user_id` | uuid |  | [`users`](users.md) | User account used by this assessor to log in.
16|`nationality_id` | uuid |  | [`countries`](countries.md) | Nationality (citizenship) of the assessor
17|`registration_method` | varchar |  |  | Self-registered or invited by Takamol. Enum.
18|`review_state` | varchar |  |  | Assessor's current state of being able to conduct assessments. Enumeration.
19|`test_center_id` | uuid |  | [`test_centers`](test_centers.md) | Test center the assessor is working from
20|`rejection_reason` | text |  |  | Reason why the assessor was rejected
21|`document_type` | varchar |  |  | TODO: Type of document that identifies the assessor. In stg v2 it's always 'passport'. As we already have passports table there is no need to store this field here
22|`international_qualifications` | varchar |  |  | TODO: One or more of: no_international_qualification, degree, diploma, training. Separated by colons. To decide - an array or a separate table
23|`full_name` | varchar |  |  | Assessor's full name.
24|`created_at` | timestamp |  |  | 
25|`updated_at` | timestamp |  |  | 
26|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record.
