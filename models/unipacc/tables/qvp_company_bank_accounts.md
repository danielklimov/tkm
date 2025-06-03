---
title: qvp_company_bank_accounts 
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
<tr><td>1</td><td>`id`</td><td>uuid</td><td>V</td><td></td><td></td></tr>
<tr><td>2</td><td>`name_en`</td><td>varchar</td><td></td><td></td><td>Display name in English</td></tr>
<tr><td>3</td><td>`swift_code`</td><td>varchar</td><td></td><td></td><td>SWIFT code (BIC) - Bank id code</td></tr>
<tr><td>4</td><td>`iban_code`</td><td>varchar</td><td></td><td></td><td>IBAN - account number</td></tr>
<tr><td>5</td><td>`qvp_company_id`</td><td>uuid</td><td></td><td>[`qvp_companies`](qvp_companies.md)</td><td>Account owner</td></tr>
<tr><td>6</td><td>`bank_account_confirmation_file_id`</td><td>uuid</td><td></td><td>[`file_storage`](file_storage.md)</td><td>Bank account confirmation file</td></tr>
<tr><td>7</td><td>`created_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>7</td><td>`created_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>8</td><td>`updated_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>8</td><td>`updated_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>9</td><td>`deleted_status`</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>
<tr><td>9</td><td>`deleted_status`</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>