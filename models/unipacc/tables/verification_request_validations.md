verification_request_validations
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION  | COMMENTS          
---|------|-----------|----|----|--------------|----------
1|`id` | uuid | V |  |  | 
2|`verification_request_id` | uudi |  | [`verification_request`](verification_request.md) | Verification request that was validated | 
3|`verification_request_type` | varchar |  |  | One of: professionalCertificate, experience, education | 
4|`invalid_fields` | text |  |  | List of invalid fields separated by commas. | Check that field names match field names in PACC.
5|`validation_ts` | timestamp |  |  | Date and time of validation. | 
6|`created_at` | timestamp |  |  |  | 
7|`updated_at` | timestamp |  |  |  | 
8|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record. | 
