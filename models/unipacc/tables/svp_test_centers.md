---
title: svp_test_centers 
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
<tr><td>1</td><td>`id`</td><td>uuid</td><td>V</td><td></td><td>autoincr</td></tr>
<tr><td>2</td><td>`name`</td><td>varchar</td><td></td><td></td><td>Test center name</td></tr>
<tr><td>3</td><td>`city`</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>4</td><td>`address`</td><td>varchar</td><td></td><td></td><td>Street address</td></tr>
<tr><td>5</td><td>`is_active`</td><td>varchar</td><td></td><td></td><td>One of: active, inactive, deleted</td></tr>
<tr><td>6</td><td>`phone_number`</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>7</td><td>`postal_code`</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>8</td><td>`user_id`</td><td>uuid</td><td></td><td>[`users`](users.md)</td><td></td></tr>
<tr><td>9</td><td>`country_id`</td><td>uuid</td><td></td><td>[`countries`](countries.md)</td><td></td></tr>
<tr><td>10</td><td>`legislator_id`</td><td>uuid</td><td></td><td>[`legislators`](legislators.md)</td><td></td></tr>
<tr><td>11</td><td>`latitude`</td><td>double</td><td></td><td></td><td>Test center location - latitude</td></tr>
<tr><td>12</td><td>`longitude`</td><td>double</td><td></td><td></td><td>Test center location - longitude</td></tr>
<tr><td>27</td><td>`created_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>27</td><td>`created_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>28</td><td>`updated_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>28</td><td>`updated_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>29</td><td>`deleted_status`</td><td>integer</td><td></td><td></td><td>0 - active record, 1 - deleted record.</td></tr>
<tr><td>29</td><td>`deleted_status`</td><td>integer</td><td></td><td></td><td>0 - active record, 1 - deleted record.</td></tr>

</table>