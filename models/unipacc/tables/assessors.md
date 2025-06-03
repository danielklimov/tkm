---
title: assessors 
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
<tr><td>1</td><td>`id`</td><td>uuid</td><td>V</td><td></td><td>Auto-generated or manually generated during migration</td></tr>
<tr><td>2</td><td>`date_of_birth`</td><td>date</td><td></td><td></td><td></td></tr>
<tr><td>3</td><td>`gender`</td><td>varchar</td><td></td><td></td><td>Male, Female or equivalents in Arabic, or nulls</td></tr>
<tr><td>4</td><td>`institute_name`</td><td>varchar</td><td></td><td></td><td>TODO: An assessor is connected with an institute (organization) in some way. Does he work in that institute as an employee? Is he certified by that institute in some way?</td></tr>
<tr><td>5</td><td>`passport_id`</td><td>uuid</td><td></td><td>[`passports`](passports.md)</td><td>Currently active passport</td></tr>
<tr><td>6</td><td>`national_id`</td><td>varchar</td><td></td><td></td><td>national id card/document number</td></tr>
<tr><td>7</td><td>`it_skills`</td><td>varchar</td><td></td><td></td><td>Information technology skills. Enum.</td></tr>
<tr><td>8</td><td>`international_experience`</td><td>varchar</td><td></td><td></td><td>International experience (years). Enum.</td></tr>
<tr><td>9</td><td>`experience`</td><td>varchar</td><td></td><td></td><td>Experience in (years) - enumeration: </td></tr>
<tr><td>10</td><td>`is_certified_assessor`</td><td>boolean</td><td></td><td></td><td>Assessors could be certified by some 3rd parties: schools, institutes, course, universitites, etc. (outside of Takamol), if during the registration assessor marks 'certified_assessor' checkbox, then the assessor must upload the experience_certificate </td></tr>
<tr><td>11</td><td>`is_online_tools_skills`</td><td>boolean</td><td></td><td></td><td>Does the assessor have skillts for online tools: Skype, MS Office, etc.</td></tr>
<tr><td>12</td><td>`is_professional_qualification`</td><td>boolean</td><td></td><td></td><td>Does the assessor have the professional qualification for occupations that he assesses.</td></tr>
<tr><td>13</td><td>`location_country_id`</td><td>uuid</td><td></td><td>[`countries`](countries.md)</td><td>The country that assessor is located in</td></tr>
<tr><td>14</td><td>`user_id`</td><td>uuid</td><td></td><td>[`users`](users.md)</td><td>User account used by this assessor to log in.</td></tr>
<tr><td>15</td><td>`nationality_id`</td><td>uuid</td><td></td><td>[`countries`](countries.md)</td><td>Nationality (citizenship) of the assessor</td></tr>
<tr><td>16</td><td>`registration_method`</td><td>varchar</td><td></td><td></td><td>Self-registered or invited by Takamol. Enum.</td></tr>
<tr><td>17</td><td>`review_state`</td><td>varchar</td><td></td><td></td><td>Assessor's current state of being able to conduct assessments. Enumeration.</td></tr>
<tr><td>18</td><td>`test_center_id`</td><td>uuid</td><td></td><td>[`test_centers`](test_centers.md)</td><td>Test center the assessor is working from</td></tr>
<tr><td>19</td><td>`rejection_reason`</td><td>text</td><td></td><td></td><td>Reason why the assessor was rejected</td></tr>
<tr><td>20</td><td>`document_type`</td><td>varchar</td><td></td><td></td><td>TODO: Type of document that identifies the assessor. In stg v2 it's always 'passport'. As we already have passports table there is no need to store this field here</td></tr>
<tr><td>21</td><td>`international_qualifications`</td><td>varchar</td><td></td><td></td><td>TODO: One or more of: no_international_qualification, degree, diploma, training. Move to a separate table.</td></tr>
<tr><td>22</td><td>`full_name`</td><td>varchar</td><td></td><td></td><td>Assessor's full name.</td></tr>
<tr><td>23</td><td>`created_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>24</td><td>`updated_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>25</td><td>`deleted_status`</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>