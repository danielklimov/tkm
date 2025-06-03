---
title: file_storage 
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
<tr><td>1</td><td>id</td><td>uuid</td><td>V</td><td></td><td>auto-generated</td></tr>
<tr><td>2</td><td>file_type</td><td>varchar</td><td></td><td></td><td>Enum. One of predefined file types. e.g. VERIFICATION_REQUEST_CERTIFICATE. It defines the table and field that reference this file. TODO: define all possible category codes.</td></tr>
<tr><td>3</td><td>name</td><td>varchar</td><td></td><td></td><td>Original file name - the name of the file when it was being uploaded. Without path.</td></tr>
<tr><td>4</td><td>size</td><td>integer</td><td></td><td></td><td>File size in bytes</td></tr>
<tr><td>5</td><td>created_by_user_id</td><td></td><td></td><td><a href="users.md">users</a></td><td>User who created the file</td></tr>
<tr><td>6</td><td>entity_id</td><td>uuid</td><td></td><td></td><td>References different tables depending on 'file_category_code' field. See file_storage_mappings for details.</td></tr>
<tr><td>7</td><td>file_path</td><td>varchar</td><td></td><td></td><td>full path to the file on oci bucket  (a.k.a "key" in oci terms)</td></tr>
<tr><td>8</td><td>created_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>9</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>10</td><td>deleted_status</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>