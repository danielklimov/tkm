verification_payment_checkout
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | autogenerated
2|`verification_request_id` | uuid |  | [`verification_request`](verification_request.md) | Verification request that is being paid for.
3|`hyperpay_code` | varchar |  |  | it is the internal HyperPay response code, we map payment statuses on these codes
4|`payment_status` | varchar |  |  | Statuses found: failed, initialized, pending, success.
5|`amount` | integer |  |  | Payment amount
6|`currency_code` | varchar |  |  | 3-letter currency code, e.g. USD
7|`payment_type_code` | varchar |  |  | One of: CARD, DB TODO: what does DB mean? Any other types?
8|`description` | varchar |  |  | Usualy contains a string 'successfully created checkout'
9|`hyper_pay_checkout_id` | varchar |  |  | Hyperpay checkout id - hyperpay is a payment provider
10|`total_tax` | integer |  |  | Tax (VAT) included into amount
11|`created_at` | timestamp |  |  | 
12|`updated_at` | timestamp |  |  | 
13|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record.
