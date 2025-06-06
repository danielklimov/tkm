---
title: exam_sessions 
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
<tr><td>1</td><td>id</td><td>uuid</td><td>V</td><td></td><td>autogen</td></tr>
<tr><td>2</td><td>start_at</td><td>timestamp</td><td></td><td></td><td>local date and time when the exam starts</td></tr>
<tr><td>3</td><td>end_at</td><td>timestamp</td><td></td><td></td><td>local date and time when the exam ends</td></tr>
<tr><td>4</td><td>location_link</td><td>varchar</td><td></td><td></td><td>URL that points to google maps that shows the location of the test center</td></tr>
<tr><td>5</td><td>seats_count</td><td>integer</td><td></td><td></td><td>Total amount of seats. We do calculate on BE side the amount available seats the next way: seats - reservations.active.count - temporary_seats.active.count</td></tr>
<tr><td>6</td><td>availble_seats_count</td><td>integer</td><td></td><td></td><td>The number of seats currently available: seats - reservations.active.count - temporary_seats.active.count</td></tr>
<tr><td>7</td><td>test_center_id</td><td>uuid</td><td></td><td><a href="test_centers-uni.md">test_centers</a></td><td></td></tr>
<tr><td>8</td><td>verification_code</td><td>varchar</td><td></td><td></td><td>Verification code is generated by PseudorandomNumberGenerator::Handler on the BE side. Labors have it in the booking ticket and show once coming to exams</td></tr>
<tr><td>9</td><td>occupation_category_id</td><td>uuid</td><td></td><td><a href="occupation_categories-uni.md">occupation_categories</a></td><td>Occupation category for which this session is assigned</td></tr>
<tr><td>10</td><td>session_status</td><td>varchar</td><td></td><td></td><td>Enum: {"in_progress"=>0,  "scheduled"=>1,  "initially_scheduled"=>2,  "completed"=>3,  "expired"=>4,  "drafted"=>5,  "assessor_withdrawn"=>6,  "canceled"=>7}</td></tr>
<tr><td>11</td><td>repeat</td><td>varchar</td><td></td><td></td><td>Enum: {"does_not_repeat"=>0, "daily"=>1, "weekly"=>2, "monthly"=>3}</td></tr>
<tr><td>12</td><td>cancellation_reason</td><td>varchar</td><td></td><td></td><td>Free text describing why the session was cancelled</td></tr>
<tr><td>13</td><td>is_reminder_sent</td><td>boolean</td><td></td><td></td><td>A reminder was sent to all examinees</td></tr>
<tr><td>14</td><td>cancelled_by_user_id</td><td>bigint</td><td></td><td><a href="users-uni.md">users</a></td><td>User that cancelled the session</td></tr>
<tr><td>15</td><td>repeat_rule_description</td><td>varchar</td><td></td><td></td><td>Free text that describes how often is the exam session held, at which time etc.</td></tr>
<tr><td>16</td><td>time_zone_name</td><td>varchar</td><td></td><td></td><td>Time zone of start_at time</td></tr>
<tr><td>17</td><td>phase_status</td><td>integer</td><td></td><td></td><td>Enum: {"phase_one"=>0, "phase_two"=>1, "phase_completed"=>2}</td></tr>
<tr><td>18</td><td>created_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>19</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>20</td><td>deleted_status</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>