employee_invites
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | 
2|`employee_id` | uuid |  | [`qvp_company_employees`](qvp_company_employees.md) | 
3|`service_provider_id` | uuid |  | [`qvp_companies`](qvp_companies.md) | 
4|`token` | varchar |  |  | Part of unique URL the employee must visit to activate his user account
5|`email` | varchar |  |  | employee email that the invitation is sent to.
6|`expire_at` | timestamp |  |  | Expiration date of the invitation.
7|`created_at` | timestamp |  |  | 
8|`updated_at` | timestamp |  |  | 
9|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record.
