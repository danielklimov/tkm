---
title: fast_track_immediate_records 
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
<tr><td>2</td><td>passport_number</td><td>varchar</td><td></td><td></td><td>Passport number of the candidate for whom this fast track record was created.</td></tr>
<tr><td>3</td><td>entity_name_en</td><td>varchar</td><td></td><td></td><td>Entity - means organization (company) that requires fast track process</td></tr>
<tr><td>4</td><td>entity_name_ar</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>5</td><td>fast_track_status</td><td>varchar</td><td></td><td></td><td>fast track status. TODO; find out what other values except 'active' there can be</td></tr>
<tr><td>6</td><td>country_id</td><td>uuid</td><td></td><td><a href="countries.md">countries</a></td><td>Country of citizenship of the user that this fast track record is created for</td></tr>
<tr><td>7</td><td>created_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>8</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>9</td><td>deleted_status</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>