---
title: fast_track_immediate_request_docs 
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
<tr><td>1</td><td>`id`</td><td>uuid</td><td>V</td><td></td><td>autogen</td></tr>
<tr><td>2</td><td>`fast_track_immediate_request_id`</td><td>uuid</td><td></td><td>[`fast_track_immediate_requests`](fast_track_immediate_requests.md)</td><td></td></tr>
<tr><td>3</td><td>`supplementary_document_id`</td><td>uuid</td><td></td><td>[`file_storage`](file_storage.md)</td><td></td></tr>
<tr><td>4</td><td>`seq_number`</td><td>integer</td><td></td><td></td><td>Sequential number of this attached document within one fast_track_immediate_request</td></tr>
<tr><td>5</td><td>`created_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>6</td><td>`updated_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>7</td><td>`deleted_status`</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>