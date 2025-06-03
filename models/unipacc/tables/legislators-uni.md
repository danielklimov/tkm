---
title: legislators 
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
<tr><td>1</td><td>id</td><td>bigint</td><td>V</td><td></td><td>autogen</td></tr>
<tr><td>2</td><td>user_id</td><td>bigint</td><td></td><td><a href="users-uni.md">users</a></td><td>The user that created or updated the record</td></tr>
<tr><td>3</td><td>name_en</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>4</td><td>name_ar</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>5</td><td>address</td><td>varchar</td><td></td><td></td><td>Street address</td></tr>
<tr><td>6</td><td>postal_code</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>7</td><td>is_active</td><td>integer</td><td></td><td></td><td>TODO: 0, 1 and 2 - what does it mean? Is it active, not active, deleted?</td></tr>
<tr><td>8</td><td>rejection_reason</td><td>text</td><td></td><td></td><td>Free text</td></tr>
<tr><td>9</td><td>city</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>10</td><td>country_id</td><td>bigint</td><td></td><td><a href="countries-uni.md">countries</a></td><td></td></tr>
<tr><td>11</td><td>show_logo</td><td>boolean</td><td></td><td></td><td></td></tr>
<tr><td>12</td><td>created_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>13</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>14</td><td>deleted_status</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>