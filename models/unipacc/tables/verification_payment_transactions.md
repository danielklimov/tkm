verification_payment_transactions
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | autogenerated
2|`verification_request_id` | uuid |  | [`verification_requests`](verification_requests.md) | 
3|`hyper_pay_payment_id` | varchar |  |  | hyper pay id for the payment 
4|`payment_status_code` | varchar |  |  | One of: communication_rejected,rejected_by_asynchronous_workflow,external_rejected,pending,success
4|`transaction_status` | varchar |  |  | One of: communication_rejected,rejected_by_asynchronous_workflow,external_rejected,pending,success
5|`payer_email` | varchar |  |  | Applicant's email
6|`payment_processing_description` | varchar |  |  | Message from payment processor: e.g. "Request successfully processed in 'Merchant in Integrator Test Mode'"
7|`payment_brand` | varchar |  |  | One of MASTER, VISA, BRAND, MADA.
8|`payment_type` | varchar |  |  | Values found: MASTER, TYPE, VISA, DB, trail, MADA, SADAD.
9|`total_amount` | numeric(18,2) |  |  | Payment amount
10|`currency` | varchar |  |  | Payment currency - 3-letter code e.g. USD
11|`code` | varchar |  |  | it is the internal HyperPay response code, we map payment statuses on these codes
12|`payer_ip_addr` | varchar |  |  | ipv4 or ipv6 - ip address from which the payment has been originated
13|`payer_ip_addr_country_id` | uuid |  | [`countries`](countries.md) | 2-letter country code of the country that maps to the ip address
14|`total_vat` | integer |  |  | VAT (amount included into amount)
15|`is_discounted` | boolean |  |  | A flag showing if the payment has a discount.
16|`created_at` | timestamp |  |  | 
17|`updated_at` | timestamp |  |  | 
18|`deleted_status` | varchar |  |  | ACTIVE, DELETED
