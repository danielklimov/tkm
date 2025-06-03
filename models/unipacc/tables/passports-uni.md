---
title: passports 
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
<tr><td>1</td><td>id</td><td>uuid</td><td>V</td><td></td><td>Auto-generated or created from source data during migration</td></tr>
<tr><td>2</td><td>first_name</td><td>varchar</td><td></td><td></td><td>First name of the passport owner</td></tr>
<tr><td>3</td><td>last_name</td><td>varchar</td><td></td><td></td><td>Last name of the passport owner</td></tr>
<tr><td>4</td><td>passport_number</td><td>varchar</td><td></td><td></td><td>Document number</td></tr>
<tr><td>5</td><td>country_id</td><td>uuid</td><td></td><td><a href="countries-uni.md">countries</a></td><td>The country that issued the passport.</td></tr>
<tr><td>6</td><td>issue_date</td><td>date</td><td></td><td></td><td>Document issue date</td></tr>
<tr><td>7</td><td>expiration_date</td><td>date</td><td></td><td></td><td>Document expiration date</td></tr>
<tr><td>8</td><td>passport_file_id</td><td>uuid</td><td></td><td><a href="file_storage-uni.md">file_storage</a></td><td>Passport photo</td></tr>
<tr><td>9</td><td>created_by_user_id</td><td>uuid</td><td></td><td><a href="users-uni.md">users</a></td><td>The user that created this record. It does not necessarily mean that this user is the owner of the passport.</td></tr>
<tr><td>10</td><td>created_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>11</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>12</td><td>deleted_status</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>