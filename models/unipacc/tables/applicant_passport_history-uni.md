---
title: applicant_passport_history 
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
<tr><td>1</td><td>id</td><td>uuid</td><td>V</td><td></td><td>Surrogate key</td></tr>
<tr><td>2</td><td>applicant_id</td><td>uuid</td><td></td><td><a href="applicants-uni.md">applicants</a></td><td>Applicant - the owner of the passport</td></tr>
<tr><td>3</td><td>passport_id</td><td>uuid</td><td></td><td><a href="passports-uni.md">passports</a></td><td>The cuurrently active passport</td></tr>
<tr><td>4</td><td>valid_from</td><td>date</td><td></td><td></td><td>The date when this record becomes active</td></tr>
<tr><td>5</td><td>created_at</td><td>timestamp</td><td></td><td></td><td>System field - date and time when the record was created</td></tr>
<tr><td>6</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td>System field - date and time when the record was modified (or created when the record is new)</td></tr>
<tr><td>7</td><td>deleted_status</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>