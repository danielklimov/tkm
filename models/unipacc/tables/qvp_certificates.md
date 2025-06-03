---
title: qvp_certificates 
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
<tr><td>1</td><td>id</td><td>uuid</td><td>V</td><td></td><td></td></tr>
<tr><td>2</td><td>applicant_id</td><td>uuid</td><td></td><td><a href="applicants.md">applicants</a></td><td>The applicant that applied for the certificate.</td></tr>
<tr><td>3</td><td>certificate_number</td><td>varchar(40)</td><td></td><td></td><td>Human-readable certificate number that is printed on the paper document.</td></tr>
<tr><td>4</td><td>certificate_file_id</td><td>uuid</td><td></td><td><a href="file_storage.md">file_storage</a></td><td>A copy of the certificate document in pdf format. File type: QVP_CERTIFICATE</td></tr>
<tr><td>5</td><td>first_name</td><td>varchar</td><td></td><td></td><td>First name as spelled in the certificate document</td></tr>
<tr><td>6</td><td>last_name</td><td>varchar</td><td></td><td></td><td>Last name as spelled in the certificate document</td></tr>
<tr><td>7</td><td>middle_name</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>8</td><td>nationality_id</td><td>uuid</td><td></td><td><a href="countries.md">countries</a></td><td>Reference to the country of citizenship (nationality) of the applicant at the time when the certificate was issued</td></tr>
<tr><td>9</td><td>passport_number</td><td>varchar</td><td></td><td></td><td>Passport number of a person that the certificate is issued to.</td></tr>
<tr><td>10</td><td>occupation_id</td><td>varchar</td><td></td><td><a href="occupations.md">occupations</a></td><td>Occupation that is being certified</td></tr>
<tr><td>11</td><td>verification_request_id</td><td>uuid</td><td></td><td><a href="verification_requests.md">verification_requests</a></td><td>The certificate was created as the result of processing this verification request</td></tr>
<tr><td>12</td><td>created_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>13</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>14</td><td>deleted_status</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>