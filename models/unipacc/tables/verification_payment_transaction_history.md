verification_payment_transaction_history
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | 
2|`hyper_pay_payment_id` | varchar |  |  | TODO: does it reference any table, e.g. verification_payment_transaction? The table is empty on stg v2, unable to check
3|`hyper_pay_response` | text |  |  | 
4|`created_at` | timestamp |  |  | 
5|`updated_at` | timestamp |  |  | 
6|`deleted_status` | varchar |  |  | ACTIVE, DELETED
