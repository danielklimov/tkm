draft_verification_request_eligibility_scores
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | 
2|`user_id` | uuid |  | [`users`](users.md) | The user for whom eligibility scores is being calculated
3|`education_score` | integer |  |  | 
4|`experience_score` | numeric |  |  | 
5|`total_score` | numeric |  |  | 
6|`created_at` | timestamp |  |  | 
7|`updated_at` | timestamp |  |  | 
8|`deleted_status` | varchar |  |  | ACTIVE, DELETED
