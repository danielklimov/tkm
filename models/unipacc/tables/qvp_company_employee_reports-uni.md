---
title: qvp_company_employee_reports 
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
<tr><td>1</td><td>id</td><td>uuid</td><td>V</td><td></td><td></td></tr>
<tr><td>2</td><td>qvp_company_employee_id</td><td>integer</td><td></td><td><a href="qvp_company_employees-uni.md">qvp_company_employees</a></td><td></td></tr>
<tr><td>3</td><td>report_file_id</td><td>uuid</td><td></td><td><a href="file_storage-uni.md">file_storage</a></td><td>TODO: it isn't referencing file_storage in stg v2 db! An error?</td></tr>
<tr><td>4</td><td>created_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>4</td><td>created_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>5</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>5</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>6</td><td>deleted_status</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>
<tr><td>6</td><td>deleted_status</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>