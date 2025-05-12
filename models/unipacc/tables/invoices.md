invoices
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | autogen
2|`payment_id` | uuid |  | [`payments`](payments.md) | Parent payment transaction that this invoice was paid with
3|`file_id` | varchar |  | [`file_storage`](file_storage.md) | A reference to the printable copy of the invoice (pdf)
4|`document_number` | varchar(40) |  |  | A human-readable invoice number.
5|`currency_code` | varchar |  |  | Currency of the amount field (3-letter currency code)
6|`total_amount` | numeric(18,2) |  |  | Invoice amount
7|`total_tax_amount` | numeric(18,2) |  |  | Total VAT included into 'amount'
8|`buyer_name` | varchar |  |  | Name of the buyer (candidate)
9|`qr_code` | text |  |  | TODO: what does this QR code contain? How it is encoded?
10|`supplier_tax_id` | varchar |  |  | Supplier's (Takamol) tax number.
11|`supplier_name` | varchar |  |  | Supplier legal name
12|`supplier_street` | varchar |  |  | Supplier address - street name
13|`supplier_location` | varchar |  |  | Supplier address - Zipcode and country name
14|`currency_convert_ratio` | numeric(18,4) |  |  | TODO: check if it's enough precision. Convertion rate from USD to SAR that is used with this invoice for accounting purposes
15|`zatca_report` | text |  |  | ZATCa is a saudi-national e-invoicing system, all invoices are generated through ZATCA. this XML is a klind of a digitally signed elevation file for the invoice. We need to migrate it
16|`created_at` | timestamp |  |  | 
17|`updated_at` | timestamp |  |  | 
18|`deleted_status` | varchar |  |  | ACTIVE, DELETED
