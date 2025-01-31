
verification_request
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | uuid | V |  | 
2|`persona` | uuid |  | [`verification_request_persona`](verification_request_persona.md) | 
3|`education` | uuid |  | [`verification_request_education`](verification_request_education.md) | 
4|`employment` | uuid |  | [`verification_request_employment`](verification_request_employment.md) | 
5|`validation` | uuid |  | [`verification_request_validation`](verification_request_validation.md) | 
6|`candidate_id` | integer |  | [`candidate`](candidate.md) | 
7|`service_provider_id` | uuid |  | [`service_provider_company`](service_provider_company.md) | 
8|`service_provider_employee_id` | integer |  | [`service_provider_employee`](service_provider_employee.md) | 
9|`service_provider_order_id` | varchar |  |  | 
10|`status` | varchar |  |  | 
11|`created_at` | timestamp |  |  | 
12|`updated_at` | timestamp |  |  | 
15|`report_file_id` | varchar |  |  | 
16|`deleted_at` | timestamp |  |  | 
18|`number_id` | integer |  |  | 
19|`random_id` | integer |  |  | 
20|`assigned_at` | timestamp |  |  | 
26|`used_discount` | boolean |  |  | 
27|`types` | json |  |  | 
28|`received_at` | timestamp |  |  | 
29|`payment_details` | json |  |  | 
30|`fast_track_major_entity_record_id` | uuid |  | [`fast_track_major_entity_record`](fast_track_major_entity_record.md) | 
31|`major_entity_id` | uuid |  | [`fast_track_major_entity_record`](fast_track_major_entity_record.md) | 
32|`other_major_entity_name` | varchar |  |  | 
33|`fast_track_immediate_record_id` | uuid |  | [`fast_track_immediate_record`](fast_track_immediate_record.md) | 
