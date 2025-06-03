---
title: verification_request_verification_types 
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
<tr><td>2</td><td>verification_request_id</td><td>uuid</td><td></td><td><a href="verification_requests-uni.md">verification_requests</a></td><td>Verification request that requires this verification type</td></tr>
<tr><td>3</td><td>verification_type</td><td>varchar</td><td></td><td></td><td>Verification type. Enum. One of: EDUCATION,PROFESSIONAL_CERTIFICATE,EXPERIENCE</td></tr>
<tr><td>4</td><td>created_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>5</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>6</td><td>deleted_status</td><td>integer</td><td></td><td></td><td>0 - active record, 1 - deleted record.</td></tr>

</table>