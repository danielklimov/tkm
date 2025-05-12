Orders
========================

The diagram represents the flow of an applicant's verification request or
an SVP booking and how both of them go into the same flow regarding payments
and invoicing process.


The Diagram
--------

![orders diagram](img/orders.png)


Description
-------------

The whole idea is that a separate entity called "Applicant's order" has been added
in order to unify separate flows for QVP and SVP processes - VRs and bookings, respectively.
An order is a usual order modelled in the same way as orders are usually modelled in online shops.

The order entity consists of two tables:

- the main table - [applicant_orders](../tables/applicant_orders.md)
- detail table - [applicant_order_items](../tables/applicant_order_items.md).

An order usually consist only one line - "Qualification verification request" or
"Skill verification". But an additional items (lines) may be added to the order, for example, "Additional fee".

An order is created either from [verification_requests](../tables/verification_requests.md)
or [svp_bookings](../tables/svp_bookings.md) and references one of these
documents as the 'parent' document.

The [payments](../tables/payments.md) is a universal payment for QVP and SVP.
The payment is created from the order and references the order as the 'parent' entity.

The [invoices](../tables/invoices.md) is also universal for QVP and SVP. The invoice is created from payment
and references the payment as the 'parent' document.
The invoice has almost the same structure as the Order with a separate [invoice_items](../tables/invoice_items) table.


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
