---
title: verification_services 
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
<tr><td>1</td><td>`id`</td><td>uuid</td><td>V</td><td></td><td>Automatically generated surrogate key.</td></tr>
<tr><td>2</td><td>`code`</td><td>varchar(40)</td><td></td><td></td><td>Human-readable code used to refer to this record.</td></tr>
<tr><td>3</td><td>`name_en`</td><td>varchar(200)</td><td></td><td></td><td>Name in English that will be printed on invoice, e.g. Verification fee, Additional fee, Test fee</td></tr>
<tr><td>4</td><td>`name_ar`</td><td>varchar(200)</td><td></td><td></td><td>Name in Arabic that will be printed on invoice, e.g. Verification fee, Additional fee, Test fee</td></tr>
<tr><td>5</td><td>`price`</td><td>numeric(18,2)</td><td></td><td></td><td>Price in USD per one unit/one service.</td></tr>
<tr><td>6</td><td>`description`</td><td>varchar(500)</td><td></td><td></td><td>Long description (English or Arabic) for technical use.</td></tr>
<tr><td>7</td><td>`created_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>8</td><td>`updated_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>9</td><td>`deleted_status`</td><td>varchar(20)</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>