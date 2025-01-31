
verification_request_sla_logs
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | integer | V |  | 
2|`request_id` | uuid |  | [`verification_request`](verification_request.md) | 
3|`user_id` | uuid |  | [`users`](users.md) | 
4|`timestamp_start` | varchar |  |  | 
5|`timestamp_stop` | varchar |  |  | 
6|`interval_seconds` | varchar |  |  | 
7|`status` | varchar |  |  | 
8|`education_id` | uuid |  | [`verification_request_education`](verification_request_education.md) | 
9|`candidate_professional_certificate_id` | uuid |  | [`verification_request_candidate_professional_certificate`](verification_request_candidate_professional_certificate.md) | 
10|`employment_experience_id` | uuid |  |  | 
