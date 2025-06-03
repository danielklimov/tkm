---
title: majors 
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
<tr><td>1</td><td>id</td><td>uuid</td><td>V</td><td></td><td>manually generated on migration from integer value</td></tr>
<tr><td>2</td><td>name_en</td><td>varchar</td><td></td><td></td><td>Name in English</td></tr>
<tr><td>3</td><td>name_ar</td><td>varchar</td><td></td><td></td><td>Name in Arabic</td></tr>
<tr><td>4</td><td>rare_in_sa</td><td>boolean</td><td></td><td></td><td>Rare in Saudi Arabia</td></tr>
<tr><td>5</td><td>is_published</td><td>boolean</td><td></td><td></td><td>Shown is web app</td></tr>
<tr><td>6</td><td>updated_by_user_id</td><td>uuid</td><td></td><td><a href="users-uni.md">users</a></td><td>The user who updated the record last time</td></tr>
<tr><td>7</td><td>created_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>8</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>9</td><td>deleted_status</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>