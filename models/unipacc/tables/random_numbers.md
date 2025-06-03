---
title: random_numbers 
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
<tr><td>1</td><td>`id`</td><td>uuid</td><td>V</td><td></td><td>Automatically generated surrogate key</td></tr>
<tr><td>2</td><td>`random_generator_code`</td><td>varchar(40)</td><td></td><td></td><td>This field is used to partition the table between different 'random generators' to be able to use several random generators for different purposes. Currently there are 3 random generators: VERIFICATIONS - used to generate numbers for both verification requests and for verification request certificates; LEGACY_QVP - migrated from random_id table from qvp.</td></tr>
<tr><td>3</td><td>`random_number`</td><td>bigint</td><td></td><td></td><td>Randomly generated number is stored here.</td></tr>
<tr><td>4</td><td>`created_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>5</td><td>`updated_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>6</td><td>`deleted_status`</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>