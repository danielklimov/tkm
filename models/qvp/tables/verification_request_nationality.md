
verification_request_nationality
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
2|`name_arabic` | varchar |  |  | Nationality name in Arabic
3|`name_english` | varchar |  |  | How a person that belongs to this nationality is caled, e.g. Kuwaiti, Peruvian etc.
4|`deleted_at` | timestamp |  |  | 
5|`key` | integer |  |  | Sort code
6|`countrycode` | varchar |  |  | 3-letter country code
7|`country_name_arabic` | varchar |  |  | Country name in English
8|`country_name_english` | varchar |  |  | Country name in Arabic
9|`is_mandated` | boolean |  |  | Verification is required for citizens of this country having any occupation (true).
10|`mandate_from_date` | timestamp |  |  | date from which is_mandated is true
11|`id` | uuid | V |  | 
12|`alpha2code` | varchar |  |  | 2-letter country code
13|`iso3code` | varchar |  |  | 
14|`iso2code` | varchar |  |  | 
15|`iso_number` | integer |  |  | 
16|`updated_by_id` | uuid |  | [`users`](users.md) | 
17|`is_active` | boolean |  |  | 
18|`created_at` | timestamp |  |  | 
19|`updated_at` | timestamp |  |  | 
