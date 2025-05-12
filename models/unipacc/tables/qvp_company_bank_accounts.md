qvp_company_bank_accounts
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | 
2|`name_en` | varchar |  |  | Display name in English
3|`swift_code` | varchar |  |  | SWIFT code (BIC) - Bank id code
4|`iban_code` | varchar |  |  | IBAN - account number
5|`qvp_company_id` | uuid |  | [`qvp_companies`](qvp_companies.md) | Account owner
6|`bank_account_confirmation_file_id` | uuid |  | [`file_storage`](file_storage.md) | Bank account confirmation file
7|`created_at` | timestamp |  |  | 
7|`created_at` | timestamp |  |  | 
8|`updated_at` | timestamp |  |  | 
8|`updated_at` | timestamp |  |  | 
9|`deleted_status` | varchar |  |  | ACTIVE, DELETED
9|`deleted_status` | varchar |  |  | ACTIVE, DELETED
