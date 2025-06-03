---
title: verification_request_verified_employment 
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
<tr><td>1</td><td>id</td><td></td><td>V</td><td></td><td>surrogate key</td></tr>
<tr><td>2</td><td>verification_request_id</td><td>uuid</td><td></td><td><a href="verification_requests-uni.md">verification_requests</a></td><td></td></tr>
<tr><td>3</td><td>employment_experience_id</td><td>uuid</td><td></td><td><a href="verification_request_employment-uni.md">verification_request_employment</a></td><td></td></tr>
<tr><td>4</td><td>created_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>5</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>6</td><td>deleted_status</td><td>integer</td><td></td><td></td><td>0 - active record, 1 - deleted record.</td></tr>

</table>