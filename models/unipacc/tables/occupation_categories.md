---
title: occupation_categories 
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
<tr><td>1</td><td>`id`</td><td>uuid</td><td>V</td><td></td><td>Auto-generated or manually assigned during migration</td></tr>
<tr><td>2</td><td>`name_en`</td><td>varchar</td><td></td><td></td><td>Name in English</td></tr>
<tr><td>3</td><td>`name_ar`</td><td>varchar</td><td></td><td></td><td>Name in Arabic</td></tr>
<tr><td>4</td><td>`code`</td><td>integer</td><td></td><td></td><td>User-defined numeric code used for sorting</td></tr>
<tr><td>5</td><td>`occupation_program_code`</td><td>varchar</td><td></td><td></td><td>Enum. One of: QVP, SVP</td></tr>
<tr><td>6</td><td>`min_years_of_experience`</td><td>integer</td><td></td><td></td><td>Minimum years of experience required for verification for any occupation under this category</td></tr>
<tr><td>7</td><td>`is_published`</td><td>boolean</td><td></td><td></td><td>Officialy available in web app</td></tr>
<tr><td>8</td><td>`svp_exam_conf`</td><td>jsonb</td><td></td><td></td><td>Exam configuration params. In use only by SVP</td></tr>
<tr><td>9</td><td>`created_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>10</td><td>`updated_at`</td><td>timestamp</td><td></td><td></td><td>date time of creation or last update</td></tr>
<tr><td>11</td><td>`deleted_status`</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>