---
title: occupations 
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
<tr><td>1</td><td>id</td><td>uuid</td><td>V</td><td></td><td>Auto-generated or manually assigned during migration</td></tr>
<tr><td>2</td><td>name_en</td><td>varchar</td><td></td><td></td><td>English name</td></tr>
<tr><td>3</td><td>name_ar</td><td>varchar</td><td></td><td></td><td>Arabic name</td></tr>
<tr><td>4</td><td>code</td><td>integer</td><td></td><td></td><td>Numeric code used for sorting</td></tr>
<tr><td>5</td><td>occupation_category_id</td><td>uuid</td><td></td><td><a href="occupation_categories-uni.md">occupation_categories</a></td><td></td></tr>
<tr><td>6</td><td>occupation_subcategory_id</td><td>uuid</td><td></td><td><a href="occupation_subcategories-uni.md">occupation_subcategories</a></td><td></td></tr>
<tr><td>7</td><td>description</td><td>varchar</td><td></td><td></td><td>Long description</td></tr>
<tr><td>8</td><td>main_tasks</td><td>text</td><td></td><td></td><td>Even longer description</td></tr>
<tr><td>9</td><td>min_education_level_id</td><td>uuid</td><td></td><td><a href="education_levels-uni.md">education_levels</a></td><td></td></tr>
<tr><td>10</td><td>occupation_program_code</td><td>varchar</td><td></td><td></td><td>One of: qvp, svp</td></tr>
<tr><td>11</td><td>requirement_group</td><td>integer</td><td></td><td></td><td>0 - unassigned, 1 or 2. There are 2 requirement groups for QVP that define logic of calculation of eligibility score.</td></tr>
<tr><td>12</td><td>is_global</td><td>boolean</td><td></td><td></td><td>If true, the occupation must be verified for all nationalities (citizenships)</td></tr>
<tr><td>13</td><td>is_any_major_degree</td><td>boolean</td><td></td><td></td><td>true if any major degree can confirm this qualification</td></tr>
<tr><td>14</td><td>is_published</td><td>boolean</td><td></td><td></td><td>occupation is available in webapp</td></tr>
<tr><td>15</td><td>is_mofa_mandated</td><td>boolean</td><td></td><td></td><td>Qualification verification for this occupation is mandated by MOFA (Ministry of Foreign Affairs).</td></tr>
<tr><td>16</td><td>is_lmh_mandated</td><td>boolean</td><td></td><td></td><td>Skill verification for this occupation is mandated by LMH.</td></tr>
<tr><td>17</td><td>created_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>18</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>19</td><td>deleted_status</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>