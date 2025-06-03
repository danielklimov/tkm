---
title: employee_invites 
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
<tr><td>2</td><td>`employee_id`</td><td>uuid</td><td></td><td>[`qvp_company_employees`](qvp_company_employees.md)</td><td></td></tr>
<tr><td>3</td><td>`service_provider_id`</td><td>uuid</td><td></td><td>[`qvp_companies`](qvp_companies.md)</td><td></td></tr>
<tr><td>4</td><td>`token`</td><td>varchar</td><td></td><td></td><td>Part of unique URL the employee must visit to activate his user account</td></tr>
<tr><td>5</td><td>`email`</td><td>varchar</td><td></td><td></td><td>employee email that the invitation is sent to.</td></tr>
<tr><td>6</td><td>`expire_at`</td><td>timestamp</td><td></td><td></td><td>Expiration date of the invitation.</td></tr>
<tr><td>7</td><td>`created_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>8</td><td>`updated_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>9</td><td>`deleted_status`</td><td>integer</td><td></td><td></td><td>0 - active record, 1 - deleted record.</td></tr>

</table>