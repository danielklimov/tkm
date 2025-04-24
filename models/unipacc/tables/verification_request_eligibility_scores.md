verification_request_eligibility_scores
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | 
2|`verification_request_id` | uuid |  | [`verification_requests`](verification_requests.md) | The 'reverse' reference to the VR that this record is referenced from.
3|`education_score` | integer |  |  | 
4|`experience_score` | numeric |  |  | 
5|`total_score` | numeric |  |  | 
6|`created_at` | timestamp |  |  | 
7|`updated_at` | timestamp |  |  | 
8|`deleted_status` | varchar |  |  | ACTIVE, DELETED
