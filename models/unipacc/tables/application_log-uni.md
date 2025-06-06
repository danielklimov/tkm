---
title: application_log 
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
<tr><td>1</td><td>id</td><td>uuid</td><td>V</td><td></td><td>autogenerated</td></tr>
<tr><td>2</td><td>type</td><td>varchar</td><td></td><td></td><td>Type of action that user performed. There is a pre-determined list of actions, e.g. requestSubmitted, requestReassign, consentWithdrawn etc.</td></tr>
<tr><td>3</td><td>user_id</td><td>uuid</td><td></td><td><a href="users-uni.md">users</a></td><td>User that performed the action</td></tr>
<tr><td>4</td><td>description</td><td>text</td><td></td><td></td><td>Textual description of the action, e.g. Verification started. Status changed from Pending to In progress</td></tr>
<tr><td>5</td><td>data</td><td>text</td><td></td><td></td><td>A JSON that contains of old and new values of changed fields of some table</td></tr>
<tr><td>6</td><td>verification_request_id</td><td>uuid</td><td></td><td></td><td>A reference to the PK of the verification_request that was changed</td></tr>
<tr><td>7</td><td>verification_request_type</td><td>varchar</td><td></td><td></td><td>A reference to the PK of the verification_request that was changed</td></tr>
<tr><td>8</td><td>verification_request_type_record_id</td><td>uuid</td><td></td><td></td><td>uuid of the source record - a PK to one of the tables that are specified in verification_request_type</td></tr>
<tr><td>9</td><td>created_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>10</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>11</td><td>deleted_status</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>