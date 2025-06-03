---
title: education_institutes 
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
<tr><td>1</td><td>id</td><td>uuid</td><td>V</td><td></td><td>Auto-generated or manually created during migration</td></tr>
<tr><td>2</td><td>name_en</td><td>varchar</td><td></td><td></td><td>Display name for this university in UI and printed documents in English</td></tr>
<tr><td>3</td><td>name_ar</td><td>varchar</td><td></td><td></td><td>Display name for this university in UI and printed documents in Arabic</td></tr>
<tr><td>4</td><td>country_id</td><td>uuid</td><td></td><td><a href="countries.md">countries</a></td><td>institute's official country of location/registration</td></tr>
<tr><td>5</td><td>state_province</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>6</td><td>city</td><td>varchar</td><td></td><td></td><td>Institute's main office location - town or city</td></tr>
<tr><td>7</td><td>street_name</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>8</td><td>building_number</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>9</td><td>zip_code</td><td>varchar</td><td></td><td></td><td>Postal (zip) code</td></tr>
<tr><td>10</td><td>is_top_institute</td><td>boolaen</td><td></td><td></td><td>This is the flag we use in the business logic, that indicates that KSA is highly interested in people who graduated from this university, thus while calculating the eligibility score of an Applicant we'll take this flag into account</td></tr>
<tr><td>11</td><td>is_additional_fees</td><td>boolean</td><td></td><td></td><td>A flag saying that this university charges additional payments for verifying the Applicant's education. Is used while calculating the fee Applicant have to pay </td></tr>
<tr><td>12</td><td>is_online_verification</td><td>boolean</td><td></td><td></td><td>A flag, saying that there's a possibility to verify Education via Internet (Web App or API)</td></tr>
<tr><td>13</td><td>online_verification_url</td><td>varchar</td><td></td><td></td><td>URL for online education verification</td></tr>
<tr><td>14</td><td>website_url</td><td>varchar</td><td></td><td></td><td>Main website URL of the institute.</td></tr>
<tr><td>15</td><td>is_published</td><td>boolean</td><td></td><td></td><td>Visible in webapp</td></tr>
<tr><td>16</td><td>updated_by_user_id</td><td>uuid</td><td></td><td><a href="users.md">users</a></td><td>The user who updated the record last time</td></tr>
<tr><td>17</td><td>created_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>18</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>19</td><td>deleted_status</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>