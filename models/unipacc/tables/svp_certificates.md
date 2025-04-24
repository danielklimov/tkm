svp_certificates
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | surrogate key
2|`applicant_id` | uuid |  | [`applicants`](applicants.md) | The applicant, the certificate was issued for
3|`country_id` | uuid |  | [`countries`](countries.md) | TODO: Country where certificate was issued?
4|`occupation_category_id` | uuid |  | [`occupation_categories`](occupation_categories.md) | TODO: the applicant is certified for all occupations from this occupation category?
5|`payment_id` | uuid |  | [`payments`](payments.md) | TODO: waiting until payments tables from QVP and SVP are refactored and posiblyunified into 1 table
6|`certificate_number` | varchar |  |  | TODO: A number that is printed on the certificate?
7|`valid_until` | timestamp |  |  | Certificate is valid until this timestamp
8|`is_free` | boolean |  |  | Free reservation feature. If the reservation was free, then the certificate was free too and it is saved here. TODO: is this field required?
9|`emailed_certificates_count` | integer |  |  | When the user clicks 'generate certificate' and the PDF is generated and email job is processed, we increase this field (+1). TODO: is this field required?
10|`access_token` | varchar |  |  | Access token is used a part of URL that is used by the user to download the certificate.
11|`created_at` | timestamp |  |  | 
12|`updated_at` | timestamp |  |  | 
13|`deleted_status` | varchar |  |  | ACTIVE, DELETED
