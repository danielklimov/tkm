---
title: qvp_company_invoice_status_history 
---

## Fields

<table style="width: 100%">
    <colgroup>
       <col span="1" style="width: 3%;"/>
       <col span="1" style="width: 12%;"/>
       <col span="1" style="width: 10%;"/>
       <col span="1" style="width: 3%;"/>
       <col span="1" style="width: 12%;"/>
       <col span="1" style="width: 60%;"/>
    </colgroup>
  <tr>
    <th>N</th>
    <th>Name</th>
    <th>Data type</th>
    <th>PK</th>
    <th>FK</th>
    <th>Description</th>
  </tr>
<tr><td>1</td><td>`id`</td><td>uuid</td><td>V</td><td></td><td>autoinc</td></tr>
<tr><td>2</td><td>`invoice_id`</td><td>uuid</td><td></td><td>[`qvp_company_invoices`](qvp_company_invoices.md)</td><td></td></tr>
<tr><td>3</td><td>`invoice_status`</td><td>varchar</td><td></td><td></td><td>one of: not_sent, paid, payment_pending, returned, waiting.</td></tr>
<tr><td>4</td><td>`valid_from`</td><td>timestamp</td><td></td><td></td><td>Date and time when invoice_status became valid</td></tr>
<tr><td>5</td><td>`created_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>5</td><td>`created_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>6</td><td>`updated_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>6</td><td>`updated_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>7</td><td>`deleted_status`</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>
<tr><td>7</td><td>`deleted_status`</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>