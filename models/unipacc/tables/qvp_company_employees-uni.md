---
title: qvp_company_employees 
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
<tr><td>1</td><td>id</td><td>uuid</td><td>V</td><td></td><td>auto generated</td></tr>
<tr><td>2</td><td>user_id</td><td>uuid</td><td></td><td><a href="users-uni.md">users</a></td><td>User account used by the employee to log in to app</td></tr>
<tr><td>3</td><td>qvp_company_id</td><td>uuid</td><td></td><td><a href="qvp_companies-uni.md">qvp_companies</a></td><td>QVP company the user works for</td></tr>
<tr><td>4</td><td>created_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>4</td><td>created_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>5</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>5</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>6</td><td>deleted_status</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>
<tr><td>6</td><td>deleted_status</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>