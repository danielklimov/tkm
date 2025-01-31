
verification_request_validation_history
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | uuid | V |  | 
2|`comment_id` | varchar |  |  | 
3|`invalid_fields` | text |  |  | 
4|`verification_request_validation_id` | uuid |  | [`verification_request_validation`](verification_request_validation.md) | 
5|`created_at` | timestamp |  |  | 
6|`deleted_at` | timestamp |  |  | 
