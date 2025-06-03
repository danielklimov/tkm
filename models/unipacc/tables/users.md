---
title: users 
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
<tr><td>2</td><td>`email`</td><td>varchar</td><td></td><td></td><td>User's email used for logging in</td></tr>
<tr><td>3</td><td>`roles`</td><td>varchar[]</td><td></td><td></td><td>Roles</td></tr>
<tr><td>4</td><td>`first_name`</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>5</td><td>`last_name`</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>6</td><td>`phone_number`</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>7</td><td>`phone_country_code_id`</td><td>uuid</td><td></td><td>[`phone_country_codes`](phone_country_codes.md)</td><td>Phone country code</td></tr>
<tr><td>8</td><td>`password`</td><td>varchar</td><td></td><td></td><td>password digest.</td></tr>
<tr><td>9</td><td>`last_active_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>10</td><td>`invalid_login_attempts`</td><td>integer</td><td></td><td></td><td></td></tr>
<tr><td>11</td><td>`two_factor_secret_key`</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>12</td><td>`is_second_factor_passed`</td><td>boolean</td><td></td><td></td><td></td></tr>
<tr><td>13</td><td>`ui_lang`</td><td>varchar</td><td></td><td></td><td>User interface language. One of: en, ar</td></tr>
<tr><td>14</td><td>`notification_lang`</td><td>varchar</td><td></td><td></td><td>Language, selected by user for receiving notifications - two-letter code. One of: en, ar</td></tr>
<tr><td>15</td><td>`created_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>16</td><td>`updated_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>17</td><td>`deleted_status`</td><td>integer</td><td></td><td></td><td>0 - active record, 1 - deleted record.</td></tr>

</table>