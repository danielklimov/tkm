---
title: verification_request_reject_reasons 
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
<tr><td>1</td><td>id</td><td>uuid</td><td>V</td><td></td><td>autoinc</td></tr>
<tr><td>2</td><td>reason_id</td><td>uuid</td><td></td><td><a href="verification_reject_reasons.md">verification_reject_reasons</a></td><td></td></tr>
<tr><td>3</td><td>request_id</td><td>uuid</td><td></td><td><a href="verification_requests.md">verification_requests</a></td><td></td></tr>
<tr><td>4</td><td>comment</td><td>text</td><td></td><td></td><td>Additional comment as to why the request was rejected</td></tr>
<tr><td>5</td><td>request_type</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>7</td><td>created_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>8</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>9</td><td>deleted_status</td><td>integer</td><td></td><td></td><td>0 - active record, 1 - deleted record.</td></tr>

</table>