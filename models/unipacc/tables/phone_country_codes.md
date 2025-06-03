---
title: phone_country_codes 
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
<tr><td>1</td><td>id</td><td>uuid</td><td>V</td><td></td><td>Initially a copy of actual country phone code, but not guaranteed to always coincide with it. Other codes may be used in special cases.</td></tr>
<tr><td>2</td><td>phone_code</td><td>varchar</td><td></td><td></td><td>Phone code or "dial-in code"</td></tr>
<tr><td>3</td><td>country_id</td><td>uuid</td><td></td><td><a href="countries.md">countries</a></td><td>The country (or primary country) that this code currently belongs to. null if not applicable</td></tr>
<tr><td>4</td><td>descr</td><td>varchar</td><td></td><td></td><td>Optional comments</td></tr>
<tr><td>5</td><td>created_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>6</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>7</td><td>deleted_status</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>