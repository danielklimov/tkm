---
title: country_qvp_statuses 
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
<tr><td>1</td><td>country_id</td><td>integer</td><td>V</td><td><a href="country.md">country</a></td><td></td></tr>
<tr><td>2</td><td>mandated_from_date</td><td>date</td><td></td><td></td><td>Date starting at which the requirement for verification is set for this country_id. If the requirement is lifted later, the record should be marked as record_status = 1 meaning it is marked as deleted.</td></tr>
<tr><td>3</td><td>created_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>4</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>5</td><td>deleted_status</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>