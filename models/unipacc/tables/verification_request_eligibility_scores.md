verification_request_eligibility_scores
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION  | COMMENTS          
---|------|-----------|----|----|--------------|----------
1|`id` | uuid | V |  | 
2|`verification_request_id` | uuid |  | [`verification_requests`](verification_requests.md) | 
3|`education_score` | integer |  |  | 
4|`experience_score` | numeric |  |  | 
5|`total_score` | numeric |  |  | 
6|`created_at` | timestamp |  |  | 
7|`updated_at` | timestamp |  |  | 
8|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record.
23|`created_at` | timestamp |  |  | 
24|`updated_at` | timestamp |  |  | 
25|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record.
