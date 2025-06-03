---
title: applicants 
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
<tr><td>1</td><td>applicant_id</td><td>uuid</td><td>V</td><td></td><td></td></tr>
<tr><td>2</td><td>user_id</td><td>uuid</td><td></td><td><a href="users.md">users</a></td><td>User account used by the applicant to log in</td></tr>
<tr><td>3</td><td>gender</td><td>varchar</td><td></td><td></td><td>One of: male, female</td></tr>
<tr><td>4</td><td>date_of_birth</td><td>date</td><td></td><td></td><td></td></tr>
<tr><td>5</td><td>country_of_residence_id</td><td>integer</td><td></td><td><a href="countries.md">countries</a></td><td>Current country of residence</td></tr>
<tr><td>6</td><td>state_province</td><td>varchar</td><td></td><td></td><td>State or province of current location (residence?)</td></tr>
<tr><td>7</td><td>phone_number</td><td>varchar</td><td></td><td></td><td>Phone number without country code</td></tr>
<tr><td>8</td><td>phone_country_code_id</td><td>integer</td><td></td><td><a href="phone_country_codes.md">phone_country_codes</a></td><td>Country id that the phone number is issued in (not the telephone country code itself).</td></tr>
<tr><td>9</td><td>email</td><td>varchar</td><td></td><td></td><td>Applicant's email.</td></tr>
<tr><td>10</td><td>first_name</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>11</td><td>middle_name</td><td>varchar</td><td></td><td></td><td>Middle name or father's name</td></tr>
<tr><td>12</td><td>last_name</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>13</td><td>maiden_name</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>14</td><td>former_married_name</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>15</td><td>mothers_name</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>16</td><td>suffix</td><td>varchar</td><td></td><td></td><td>Suffix that goes after last_name, like Ph.D.</td></tr>
<tr><td>17</td><td>passport_id</td><td>uuid</td><td></td><td><a href="passports.md">passports</a></td><td>Currently active passport. A historical attribute. When its value changes, old value is stored in applicant_passport_history table</td></tr>
<tr><td>18</td><td>fast_track_record_id</td><td>uuid</td><td></td><td><a href="fast_track_immediate_record.md">fast_track_immediate_record</a></td><td>Reference to the fast track record that was created for this applicant</td></tr>
<tr><td>19</td><td>is_auto_registered</td><td>boolean</td><td></td><td></td><td>true if the record was created for this person automatically without the applicant interaction.</td></tr>
<tr><td>20</td><td>created_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>21</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>22</td><td>deleted_status</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>