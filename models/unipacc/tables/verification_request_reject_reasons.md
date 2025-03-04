verification_request_reject_reasons
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION  | COMMENTS          
---|------|-----------|----|----|--------------|----------
1|`id` | uuid | V |  | autoinc
2|`reason_id` | uuid |  | [`verification_reject_reasons`](verification_reject_reasons.md) | 
3|`request_id` | uuid |  | [`verification_requests`](verification_requests.md) | 
4|`comment` | text |  |  | Additional comment as to why the request was rejected
5|`created_at` | timestamp |  |  | 
6|`updated_at` | timestamp |  |  | 
7|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record.
