
assessor_confirmations
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | uuid | V |  | surrogate key
2|`email_confirmation_code` | varchar |  |  | 
3|`phone_confirmation_code` | varchar |  |  | 
4|`email_confirmed` | boolean |  |  | 
5|`phone_confirmed` | boolean |  |  | 
6|`email_confirmation_send_at` | timestamp |  |  | 
7|`phone_confirmation_send_at` | timestamp |  |  | 
8|`created_at` | timestamp |  |  | 
9|`updated_at` | timestamp |  |  | 
