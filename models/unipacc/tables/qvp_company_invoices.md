---
title: qvp_company_invoices 
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
<tr><td>1</td><td>id</td><td>uuid</td><td>V</td><td></td><td>autogen</td></tr>
<tr><td>2</td><td>message</td><td>varchar</td><td></td><td></td><td>The message that is sent by SP to Takamol admin along with the invoice </td></tr>
<tr><td>3</td><td>file_id</td><td>varchar</td><td></td><td><a href="file_storage.md">file_storage</a></td><td>A printable version of the invoice</td></tr>
<tr><td>4</td><td>invoice_status</td><td>varchar</td><td></td><td></td><td>one of: not_sent, paid, payment_pending, returned, waiting</td></tr>
<tr><td>5</td><td>created_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>6</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>7</td><td>deleted_status</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>