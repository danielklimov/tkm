Orders
========================

The diagram represents the process of applicant's 'ordering' Takamol verification services,
paying for them, and receiving the invoice.


The Diagram
------------

![orders diagram](img/orders.png)


Description
-------------

A new entity - "Applicant's order" has been added
to unify ordering and payments for two separate document flows - QVP verification requests and SVP bookings.
Order can be thought of as a replacement for `payment_checkout` table in QVP.

The data model for orders follows the same design pattern as orders/invoices are usually modelled in
online businesses.

The order entity consists of two tables:

- the main table (header) - [applicant_orders](../tables/applicant_orders.md)
- order items or 'lines' - [applicant_order_items](../tables/applicant_order_items.md).

An order usually consist of only one line - "Qualification verification request" or
"Skill verification exam". But an additional items (lines) may be added, for example, "Additional fee".

An order item references another new table - [verification_services](../tables/verification_services.md).
This table acts as a 'products' table and will contain only 3 records:

1. Qualification verification request
2. Skill verification exam
3. Additional fee for qualification verification

with possibility to add more services in future.

The order is created from [verification_requests](../tables/verification_requests.md)
or [svp_bookings](../tables/svp_bookings.md) and it references one of these
documents as the 'parent' document. There are two fields for that:

- parent_document_type - one of VERIFICATION_REQUEST, SVP_BOOKING
- parent_document_id - uuid referencing either `verification_requests` or `svp_bookings`.

The [payments](../tables/payments.md) is a universal payment for QVP and SVP.
The payment is created from the order and references the order as the 'parent' entity.

The [invoices](../tables/invoices.md) is also universal for QVP and SVP. The invoice is created from payment
and references the payment as the 'parent' document.
The invoice has almost the same structure as the Order with a separate [invoice_items](../tables/invoice_items) table.

Orders are an extension to `verification_requests` and `svp_bookings`, adding
common behavior to both these tables and describing the ordering process in standardized terms.


All Tables in the Diagram
---------------------------

### QVP and SVP Requests ###

- [verification_requests](../tables/verification_requests.md)  
- [svp_bookings](../tables/svp_bookings.md)  


### Orders ###

- [applicant_orders](../tables/applicant_orders.md)  
- [applicant_order_items](../tables/applicant_order_items.md)  

### Products ###

- [verification_services](../tables/verification_services.md)  

### Payments ###

- [payments](../tables/payments.md)  

### Invoices ###

- [invoices](../tables/invoices.md)  
- [invoice_items](../tables/invoice_items.md)  
