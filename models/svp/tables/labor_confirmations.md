
labor_confirmations
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | uuid | V |  | 
2|`email_confirmation_code` | varchar |  |  | 
3|`phone_confirmation_code` | varchar |  |  | 
4|`email_confirmed` | boolean |  |  | 
5|`phone_confirmed` | boolean |  |  | 
6|`created_at` | timestamp |  |  | 
7|`updated_at` | timestamp |  |  | 
8|`email_confirmation_send_at` | timestamp |  |  | 
9|`phone_confirmation_send_at` | timestamp |  |  | 
