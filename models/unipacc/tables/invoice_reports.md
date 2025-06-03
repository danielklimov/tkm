---
title: invoice_reports 
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
<tr><td>1</td><td>`id`</td><td>uuid</td><td>V</td><td></td><td>autoincrement</td></tr>
<tr><td>2</td><td>`hyper_pay_payment_id`</td><td>varchar</td><td></td><td></td><td>HyperPay internal payment id</td></tr>
<tr><td>3</td><td>`status`</td><td>varchar</td><td></td><td></td><td>payment status: on of: PENDING, SUCCEEDED</td></tr>
<tr><td>4</td><td>`created_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>4</td><td>`created_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>5</td><td>`invoice_type`</td><td>varchar</td><td></td><td></td><td>So far all records contain one value - 'invoice'. Lets keep it. Although RN we only have invoices for VRs, later we might have sub-invoices for extra payments, this is where we'll be able to specify types</td></tr>
<tr><td>7</td><td>`updated_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>8</td><td>`deleted_status`</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>