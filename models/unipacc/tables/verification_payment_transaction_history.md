---
title: verification_payment_transaction_history 
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
<tr><td>1</td><td>`id`</td><td>uuid</td><td>V</td><td></td><td></td></tr>
<tr><td>2</td><td>`hyper_pay_payment_id`</td><td>varchar</td><td></td><td></td><td>TODO: does it reference any table, e.g. verification_payment_transaction? The table is empty on stg v2, unable to check</td></tr>
<tr><td>3</td><td>`hyper_pay_response`</td><td>text</td><td></td><td></td><td></td></tr>
<tr><td>4</td><td>`created_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>5</td><td>`updated_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>6</td><td>`deleted_status`</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>