---
title: prometric_question_logs 
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
<tr><td>1</td><td>`id`</td><td>uuid</td><td>V</td><td></td><td>autoincrement</td></tr>
<tr><td>2</td><td>`name`</td><td>varchar</td><td></td><td></td><td>Exam name</td></tr>
<tr><td>3</td><td>`question_type`</td><td>varchar</td><td></td><td></td><td>Type of question. So far only one type was found - MultipleChoice.</td></tr>
<tr><td>4</td><td>`correct_answer`</td><td>varchar</td><td></td><td></td><td>Correct option(s), e.g.: A, D, DEF, </td></tr>
<tr><td>5</td><td>`score_min`</td><td>integer</td><td></td><td></td><td>Minimum possible score - always 0</td></tr>
<tr><td>6</td><td>`score_max`</td><td>integer</td><td></td><td></td><td>Maximum score 1 or greater. E.g. if there are 3 correct answers, max score is 3</td></tr>
<tr><td>7</td><td>`category_name`</td><td>varchar</td><td></td><td></td><td>Always empty.</td></tr>
<tr><td>8</td><td>`created_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>9</td><td>`updated_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>10</td><td>`deleted_status`</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>