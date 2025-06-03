---
title: draft_verification_request_eligibility_scores 
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
<tr><td>2</td><td>`user_id`</td><td>uuid</td><td></td><td>[`users`](users.md)</td><td>The user for whom eligibility scores is being calculated</td></tr>
<tr><td>3</td><td>`education_score`</td><td>integer</td><td></td><td></td><td></td></tr>
<tr><td>4</td><td>`experience_score`</td><td>numeric</td><td></td><td></td><td></td></tr>
<tr><td>5</td><td>`total_score`</td><td>numeric</td><td></td><td></td><td></td></tr>
<tr><td>6</td><td>`created_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>7</td><td>`updated_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>8</td><td>`deleted_status`</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>