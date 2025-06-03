---
title: exam_results 
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
<tr><td>1</td><td>`id`</td><td>uuid</td><td>V</td><td></td><td>Autoincr</td></tr>
<tr><td>2</td><td>`svp_booking_id`</td><td>uuid</td><td></td><td>[`svp_bookings`](svp_bookings.md)</td><td>A link with the booking for this exam</td></tr>
<tr><td>3</td><td>`original_cbt_score`</td><td>integer</td><td></td><td></td><td>CBT score as is, without corrections</td></tr>
<tr><td>4</td><td>`original_practical_score`</td><td>integer</td><td></td><td></td><td>Practical score as is, without corrections</td></tr>
<tr><td>5</td><td>`calculated_cbt_score`</td><td>integer</td><td></td><td></td><td>CNT exam score after corrections</td></tr>
<tr><td>6</td><td>`calculated_practical_score`</td><td>integer</td><td></td><td></td><td>Practical score after corrections</td></tr>
<tr><td>7</td><td>`response_id`</td><td>varchar</td><td></td><td></td><td>The "identity" value from The Prometric outcome response</td></tr>
<tr><td>8</td><td>`practical_response_id`</td><td>varchar</td><td></td><td></td><td>The "identity" value from The Prometric outcome response (practical exam)</td></tr>
<tr><td>9</td><td>`created_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>10</td><td>`updated_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>11</td><td>`deleted_status`</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>