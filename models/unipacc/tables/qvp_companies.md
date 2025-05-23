qvp_companies
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | autogenerated
2|`name_en` | varchar |  |  | Display name in English
3|`name_ar` | varchar |  |  | Display name in Arabic
4|`country_id` | uuid |  | [`countries`](countries.md) | 
5|`registration_number` | varchar |  |  | Tax (registration) number of the company in the country where it is registered
6|`last_verification_request_assign_date` | timestamp |  |  | Statistics: last (the latest) date when a verification request was assigned to this service provider
7|`is_ready` | boolean |  |  | TODO: what does 'ready' mean in this context? is_active? Show it in webapp?
8|`legal_name` | varchar |  |  | Legal name of the company
9|`kse_license_number` | varchar |  |  | A license issued by KSE to the company's own country to perform verification services?
10|`kse_license_issuing_date` | date |  |  | 
11|`kse_license_end_date` | date |  |  | 
12|`email` | varchar |  |  | 
13|`phone_number` | varchar |  |  | Phone number without country code
14|`phone_country_code_id` | varchar |  | [`phone_country_codes`](phone_country_codes.md) | Country code for phone_number
15|`additional_phone_number` | varchar |  |  | Additional telephone number
16|`additional_phone_country_code_id` | varchar |  | [`phone_country_codes`](phone_country_codes.md) | 
17|`website_url` | varchar |  |  | 
18|`building_number` | varchar |  |  | 
19|`street_name` | varchar |  |  | 
20|`neighborhood` | varchar |  |  | 
21|`city` | varchar |  |  | 
22|`postal_code` | varchar |  |  | 
24|`bank_account_holder_name` | varchar |  |  | Company name as must be used in payment documents
25|`is_filled` | boolean |  |  | TODO: not sure what does that mean but there are records with both true and false, so probably it is still in use
26|`agreed_on_terms_and_conditions` | boolean |  |  | The service provider company has agreed on terms and conditions by Takamol
27|`license_document_file_id` | varchar |  | [`file_storage`](file_storage.md) | A reference to a file that contains the company's license.
28|`company_status` | varchar |  |  | Current status of the company. One of: active, deactivated, suspended.
29|`is_internal` | boolean |  |  | There are SPs considered as internal, thus belonging to Takamol holding. They can verify some specific requests, this bool is used to ensure the correct work of the Load balancer
30|`created_at` | timestamp |  |  | 
31|`updated_at` | timestamp |  |  | 
32|`deleted_status` | varchar |  |  | ACTIVE, DELETED
