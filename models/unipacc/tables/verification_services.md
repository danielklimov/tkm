verification_services
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | Automatically generated surrogate key.
2|`code` | varchar(40) |  |  | Human-readable code used to refer to this record.
3|`name_en` | varchar(200) |  |  | Name in English that will be printed on invoice, e.g. Verification fee, Additional fee, Test fee
4|`name_ar` | varchar(200) |  |  | Name in Arabic that will be printed on invoice, e.g. Verification fee, Additional fee, Test fee
5|`price` | numeric(18,2) |  |  | Price in USD per one unit/one service.
6|`description` | varchar(500) |  |  | Long description (English or Arabic) for technical use.
7|`created_at` | timestamp |  |  | 
8|`updated_at` | timestamp |  |  | 
9|`deleted_status` | varchar(20) |  |  | ACTIVE, DELETED
