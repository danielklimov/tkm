education_institutes
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | Auto-generated or manually created during migration
2|`name_en` | varchar |  |  | Display name for this university in UI and printed documents in English
3|`name_ar` | varchar |  |  | Display name for this university in UI and printed documents in Arabic
4|`country_id` | uuid |  | [`countries`](countries.md) | institute's official country of location/registration
5|`state_province` | varchar |  |  | 
6|`city` | varchar |  |  | Institute's main office location - town or city
7|`street_name` | varchar |  |  | 
8|`building_number` | varchar |  |  | 
9|`zip_code` | varchar |  |  | Postal (zip) code
10|`is_top_institute` | boolaen |  |  | This is the flag we use in the business logic, that indicates that KSA is highly interested in people who graduated from this university, thus while calculating the eligibility score of an Applicant we'll take this flag into account
11|`is_additional_fees` | boolean |  |  | A flag saying that this university charges additional payments for verifying the Applicant's education. Is used while calculating the fee Applicant have to pay 
12|`is_online_verification` | boolean |  |  | A flag, saying that there's a possibility to verify Education via Internet (Web App or API)
13|`online_verification_url` | varchar |  |  | URL for online education verification
14|`website_url` | varchar |  |  | Main website URL of the institute.
15|`is_published` | boolean |  |  | Visible in webapp
16|`updated_by_user_id` | uuid |  | [`users`](users.md) | The user who updated the record last time
17|`created_at` | timestamp |  |  | 
18|`updated_at` | timestamp |  |  | 
19|`deleted_status` | varchar |  |  | ACTIVE, DELETED
