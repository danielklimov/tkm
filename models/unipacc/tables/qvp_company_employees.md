qvp_company_employees
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION  | COMMENTS          
---|------|-----------|----|----|--------------|----------
1|`id` | uuid | V |  | auto generated | 
2|`user_id` | uuid |  | [`users`](users.md) | User account used by the employee to log in to app | 
3|`qvp_company_id` | uuid |  | [`qvp_companies`](qvp_companies.md) | QVP company the user works for | 
4|`created_at` | timestamp |  |  |  | 
5|`updated_at` | timestamp |  |  |  | 
6|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record. | 
18|`created_at` | timestamp |  |  |  | 
19|`updated_at` | timestamp |  |  |  | 
20|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record. | 
