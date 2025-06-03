---
title: fast_track_major_entity_requests 
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
<tr><td>1</td><td>id</td><td>uuid</td><td>V</td><td></td><td>autogen</td></tr>
<tr><td>2</td><td>created_by_user_id</td><td>uuid</td><td></td><td><a href="users-uni.md">users</a></td><td></td></tr>
<tr><td>3</td><td>updated_by_user_id</td><td>uuid</td><td></td><td><a href="users-uni.md">users</a></td><td></td></tr>
<tr><td>4</td><td>entity_name_en</td><td>varchar</td><td></td><td></td><td>Entity that submitted the request</td></tr>
<tr><td>5</td><td>entity_name_ar</td><td>varchar</td><td></td><td></td><td>Entity that submitted the request</td></tr>
<tr><td>6</td><td>supplementary_document_ids</td><td>text</td><td></td><td></td><td>TODO: strings encoded like this: a:1:{i:0;s:36:"627430b0-d398-4a7c-831e-f02a0ec532d7";}</td></tr>
<tr><td>7</td><td>start_date</td><td>timestamp</td><td></td><td></td><td>The fast track may have the dates when it becomes effective and when it expires</td></tr>
<tr><td>8</td><td>end_date</td><td>timestamp</td><td></td><td></td><td>The fast track may have the dates when it becomes effective and when it expires</td></tr>
<tr><td>9</td><td>request_status</td><td>varchar</td><td></td><td></td><td>one of: submitted, pending_updates, approved, rejected</td></tr>
<tr><td>10</td><td>comment</td><td>text</td><td></td><td></td><td>Free text</td></tr>
<tr><td>11</td><td>major_entity_number</td><td>varchar</td><td></td><td></td><td>I believe initially it was planned that there will be a separate table with major entities (4 entities exist rn), but seems it was not implemented. However, I'm thinking about keeping the standalone table for it  wit</td></tr>
<tr><td>12</td><td>created_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>13</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>14</td><td>deleted_status</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>