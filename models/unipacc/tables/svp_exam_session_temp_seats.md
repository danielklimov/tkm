---
title: svp_exam_session_temp_seats 
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
<tr><td>1</td><td>id</td><td>uuid</td><td>V</td><td></td><td>autoincrement</td></tr>
<tr><td>2</td><td>expired_at</td><td>timestamp</td><td></td><td></td><td>The expiration time of temporarily seats (the temporarilly seat is created for 20 minutes allowing user to make a payment for a reservation)</td></tr>
<tr><td>3</td><td>exam_session_id</td><td>uuid</td><td></td><td><a href="exam_sessions.md">exam_sessions</a></td><td>Exam session where the reservation is going to be made</td></tr>
<tr><td>4</td><td>applicant_id</td><td>uuid</td><td></td><td><a href="applicants.md">applicants</a></td><td>Labor who is creating a reservation.</td></tr>
<tr><td>5</td><td>created_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>5</td><td>created_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>6</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>6</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>7</td><td>deleted_status</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>
<tr><td>7</td><td>deleted_status</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>