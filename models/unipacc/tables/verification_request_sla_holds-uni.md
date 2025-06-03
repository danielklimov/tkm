---
title: verification_request_sla_holds 
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
<tr><td>2</td><td>request_id</td><td>uuid</td><td></td><td><a href="verification_requests-uni.md">verification_requests</a></td><td>VR that caused this hold</td></tr>
<tr><td>3</td><td>education_id</td><td>uuid</td><td></td><td><a href="verification_request_education-uni.md">verification_request_education</a></td><td>Education record that caused a hold</td></tr>
<tr><td>4</td><td>profeccional_certificate_id</td><td>uuid</td><td></td><td><a href="verification_request_professional_certificates-uni.md">verification_request_professional_certificates</a></td><td>Professional certificate record that caused a hold</td></tr>
<tr><td>5</td><td>employment_experience_id</td><td>uuid</td><td></td><td><a href="verification_request_employment-uni.md">verification_request_employment</a></td><td>Employment record that caused a hold</td></tr>
<tr><td>6</td><td>user_id</td><td>uuid</td><td></td><td><a href="users-uni.md">users</a></td><td>User that created a hold</td></tr>
<tr><td>7</td><td>start_ts</td><td>long</td><td></td><td></td><td>unix epoch (ms since 1 jan 1970)</td></tr>
<tr><td>8</td><td>stop_ts</td><td>long</td><td></td><td></td><td>unix epoch (ms since 1 jan 1970)</td></tr>
<tr><td>9</td><td>hold_duration_secs</td><td>long</td><td></td><td></td><td>Hold duration in seconds</td></tr>
<tr><td>10</td><td>hold_status</td><td>varchar</td><td></td><td></td><td>one of: on_hold, in_progress</td></tr>
<tr><td>11</td><td>reason</td><td>varchar</td><td></td><td></td><td>Arbitrary string e.g. 'Educational institute does not respond'</td></tr>
<tr><td>12</td><td>description</td><td>text</td><td></td><td></td><td>Detailed description of the hold</td></tr>
<tr><td>13</td><td>revoke_comment</td><td>varchar</td><td></td><td></td><td>Arbitrary string - a description of how/why the hold was revoked</td></tr>
<tr><td>14</td><td>previous_status</td><td>varchar</td><td></td><td></td><td>Previous status of verification_request, that is, the status of VR at the moment when the hold was created</td></tr>
<tr><td>15</td><td>created_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>16</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>17</td><td>deleted_status</td><td>integer</td><td></td><td></td><td>0 - active record, 1 - deleted record.</td></tr>

</table>