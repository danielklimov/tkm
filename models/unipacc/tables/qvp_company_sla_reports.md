---
title: qvp_company_sla_reports 
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
<tr><td>1</td><td>`id`</td><td>uuid</td><td>V</td><td></td><td>autogen</td></tr>
<tr><td>2</td><td>`qvp_company_id`</td><td>uuid</td><td></td><td>[`qvp_companies`](qvp_companies.md)</td><td></td></tr>
<tr><td>3</td><td>`done_requests`</td><td>integer</td><td></td><td></td><td>Total number of completed verification requests</td></tr>
<tr><td>4</td><td>`average_days`</td><td>integer</td><td></td><td></td><td>Average days per verification of 1 verification request</td></tr>
<tr><td>5</td><td>`verification_request_type`</td><td>varchar</td><td></td><td></td><td>Type of verification request: 'education', 'experiene', 'professional certificate'. </td></tr>
<tr><td>6</td><td>`created_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>7</td><td>`updated_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>8</td><td>`deleted_status`</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>