---
title: verification_request_personas 
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
<tr><td>2</td><td>first_name</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>3</td><td>last_name</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>4</td><td>middle_name</td><td>varchar</td><td></td><td></td><td>Middle name or father's name</td></tr>
<tr><td>5</td><td>gender</td><td>varchar</td><td></td><td></td><td>One of: 'Female', 'Male'</td></tr>
<tr><td>6</td><td>date_of_birth</td><td>date</td><td></td><td></td><td></td></tr>
<tr><td>7</td><td>nationality_id</td><td>uuid</td><td></td><td><a href="countries-uni.md">countries</a></td><td>Country of nationality (citizenship).</td></tr>
<tr><td>8</td><td>passport_id</td><td>uuid</td><td></td><td><a href="passport-uni.md">passport</a></td><td>User's current passport.</td></tr>
<tr><td>9</td><td>country_of_residence_id</td><td>uuid</td><td></td><td><a href="countries-uni.md">countries</a></td><td>User's current country of residence (location).</td></tr>
<tr><td>10</td><td>state_province</td><td>varchar</td><td></td><td></td><td>State or province of current location (residence?)</td></tr>
<tr><td>11</td><td>created_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>12</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>13</td><td>deleted_status</td><td>integer</td><td></td><td></td><td>0 - active record, 1 - deleted record.</td></tr>

</table>