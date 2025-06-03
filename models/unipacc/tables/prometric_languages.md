---
title: prometric_languages 
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
<tr><td>1</td><td>`id`</td><td>uuid</td><td>V</td><td></td><td>uuid(language_code)</td></tr>
<tr><td>2</td><td>`language_code`</td><td>varchar</td><td></td><td></td><td>Two-letter language code</td></tr>
<tr><td>3</td><td>`name_ar`</td><td>varchar</td><td></td><td></td><td>Name in Arabic</td></tr>
<tr><td>4</td><td>`name_en`</td><td>varchar</td><td></td><td></td><td>Name in English</td></tr>
<tr><td>5</td><td>`is_active`</td><td>boolean</td><td></td><td></td><td>Available for selection</td></tr>
<tr><td>6</td><td>`created_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>7</td><td>`updated_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>8</td><td>`deleted_status`</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>