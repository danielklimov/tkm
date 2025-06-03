---
title: qvp_company_reports 
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
<tr><td>2</td><td>`company_id`</td><td>uuid</td><td></td><td>[`qvp_companies`](qvp_companies.md)</td><td>QVP service provider company</td></tr>
<tr><td>2</td><td>`qvp_company_id`</td><td>uuid</td><td></td><td>[`qvp_companies`](qvp_companies.md)</td><td>QVP service provider company</td></tr>
<tr><td>3</td><td>`report_status`</td><td>varchar</td><td></td><td></td><td>Status of the report. One of: accepted, waiting.</td></tr>
<tr><td>4</td><td>`file_id`</td><td>varchar</td><td></td><td>[`file_storage`](file_storage.md)</td><td>A reference to file_storage table.</td></tr>
<tr><td>5</td><td>`invoice_id`</td><td>uuid</td><td></td><td>[`qvp_company_invoices`](qvp_company_invoices.md)</td><td>An invoice that this report is attached to.</td></tr>
<tr><td>6</td><td>`created_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>7</td><td>`updated_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>8</td><td>`deleted_status`</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>
<tr><td>23</td><td>`dasdasd`</td><td>asdas</td><td>dasda</td><td>[`dasd`](dasd.md)</td><td></td></tr>

</table>