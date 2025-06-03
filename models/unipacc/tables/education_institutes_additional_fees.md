---
title: education_institutes_additional_fees 
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
<tr><td>1</td><td>`id`</td><td>uuid</td><td>V</td><td></td><td></td></tr>
<tr><td>2</td><td>`education_institute_id`</td><td>uuid</td><td></td><td>[`education_institutes`](education_institutes.md)</td><td></td></tr>
<tr><td>3</td><td>`education_level_id`</td><td>uuid</td><td></td><td>[`education_levels`](education_levels.md)</td><td></td></tr>
<tr><td>4</td><td>`major_id`</td><td>integer</td><td></td><td>[`majors`](majors.md)</td><td></td></tr>
<tr><td>5</td><td>`updated_by_user_id`</td><td>uuid</td><td></td><td>[`users`](users.md)</td><td></td></tr>
<tr><td>6</td><td>`fee_amount`</td><td>numeric(18,2)</td><td></td><td></td><td>Fee amount in USD</td></tr>
<tr><td>7</td><td>`is_published`</td><td>boolean</td><td></td><td></td><td>Show this record in web interface and use it in business logic</td></tr>
<tr><td>8</td><td>`ministry_id`</td><td>varchar</td><td></td><td></td><td>An id in xls file from the Ministry</td></tr>
<tr><td>9</td><td>`created_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>10</td><td>`updated_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>11</td><td>`deleted_status`</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>