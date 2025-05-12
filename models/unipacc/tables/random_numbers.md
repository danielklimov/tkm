random_numbers
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | Automatically generated surrogate key
2|`random_generator_code` | varchar(40) |  |  | This field is used to partition the table between different 'random generators' to be able to use
several random generators for different purposes. Currently there are 3 random generators:
VERIFICATIONS - used to generate numbers for both verification requests and for verification request certificates;
LEGACY_QVP - migrated from random_id table from qvp.
3|`random_number` | bigint |  |  | Randomly generated number is stored here.
4|`created_at` | timestamp |  |  | 
5|`updated_at` | timestamp |  |  | 
6|`deleted_status` | varchar |  |  | ACTIVE, DELETED
