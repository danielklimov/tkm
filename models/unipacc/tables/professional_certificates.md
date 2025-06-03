---
title: professional_certificates 
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
<tr><td>2</td><td>name_en</td><td>varchar</td><td></td><td></td><td>certificate name in English</td></tr>
<tr><td>3</td><td>name_ar</td><td>varchar</td><td></td><td></td><td>certificate name in Arabic</td></tr>
<tr><td>4</td><td>institute_name_en</td><td>varchar</td><td></td><td></td><td>Institute or organization that issues the certificate</td></tr>
<tr><td>5</td><td>institute_name_ar</td><td>varchar</td><td></td><td></td><td>Institute or organization that issues the certificate</td></tr>
<tr><td>6</td><td>is_online_verification</td><td>boolean</td><td></td><td></td><td>Possible to check the certificate online</td></tr>
<tr><td>7</td><td>online_verification_url</td><td>varchar</td><td></td><td></td><td>URL that points to certification institute website</td></tr>
<tr><td>8</td><td>is_published</td><td>boolean</td><td></td><td></td><td>shown in webapp</td></tr>
<tr><td>9</td><td>updated_by</td><td>uuid</td><td></td><td><a href="users.md">users</a></td><td></td></tr>
<tr><td>10</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>10</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>11</td><td>deleted_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>12</td><td>created_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>14</td><td>deleted_status</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>