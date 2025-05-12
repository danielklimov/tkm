svp_certificates
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | surrogate key
2|`applicant_id` | uuid |  | [`applicants`](applicants.md) | The applicant, the certificate was issued for
3|`certificate_number` | varchar |  |  | The number that is printed on the certificate
3|`country_id` | uuid |  | [`countries`](countries.md) | TODO: Country where certificate was issued?
4|`occupation_category_id` | uuid |  | [`occupation_categories`](occupation_categories.md) | TODO: the applicant is certified for all occupations from this occupation category?
4|`certificate_file_id` | uuid |  | [`file_storage`](file_storage.md) | A copy of the certificate document in pdf format. file_type=SVP_CERTIFICATE
5|`first_name` | varchar |  |  | First name as spelled in the certificate document
5|`payment_id` | uuid |  | [`payments`](payments.md) | TODO: waiting until payments tables from QVP and SVP are refactored and posiblyunified into 1 table
6|`last_name` | varchar |  |  | Last name as spelled in the certificate document
7|`middle_name` | varchar |  |  | Middle name
8|`is_free` | boolean |  |  | Free reservation feature. If the reservation was free, then the certificate was free too and it is saved here. TODO: is this field required?
8|`nationality_id` | uuid |  | [`countries`](countries.md) | Reference to the country of citizenship (nationality) of the applicant at the time when the certificate was issued
9|`emailed_certificates_count` | integer |  |  | When the user clicks 'generate certificate' and the PDF is generated and email job is processed, we increase this field (+1). TODO: is this field required?
9|`passport_number` | varchar |  |  | Passport number of a person that the certificate is issued to.
10|`access_token` | varchar |  |  | Access token is used a part of URL that is used by the user to download the certificate.
10|`occupation_id` | uuid |  | [`occupations`](occupations.md) | Certified occupation
11|`svp_booking_id` |  |  | [`svp_bookings`](svp_bookings.md) | Reference to the initial exam booking
12|`valid_until` | timestamp |  |  | Certificate is valid until this timestamp
13|`created_at` | timestamp |  |  | 
14|`updated_at` | timestamp |  |  | 
15|`deleted_status` | varchar |  |  | ACTIVE, DELETED
