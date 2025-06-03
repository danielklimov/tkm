---
title: svp_certificates 
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
<tr><td>1</td><td>id</td><td>uuid</td><td>V</td><td></td><td>surrogate key</td></tr>
<tr><td>2</td><td>applicant_id</td><td>uuid</td><td></td><td><a href="applicants.md">applicants</a></td><td>The applicant, the certificate was issued for</td></tr>
<tr><td>3</td><td>certificate_number</td><td>varchar</td><td></td><td></td><td>The number that is printed on the certificate</td></tr>
<tr><td>3</td><td>country_id</td><td>uuid</td><td></td><td><a href="countries.md">countries</a></td><td>TODO: Country where certificate was issued?</td></tr>
<tr><td>4</td><td>occupation_category_id</td><td>uuid</td><td></td><td><a href="occupation_categories.md">occupation_categories</a></td><td>TODO: the applicant is certified for all occupations from this occupation category?</td></tr>
<tr><td>4</td><td>certificate_file_id</td><td>uuid</td><td></td><td><a href="file_storage.md">file_storage</a></td><td>A copy of the certificate document in pdf format. file_type=SVP_CERTIFICATE</td></tr>
<tr><td>5</td><td>first_name</td><td>varchar</td><td></td><td></td><td>First name as spelled in the certificate document</td></tr>
<tr><td>5</td><td>payment_id</td><td>uuid</td><td></td><td><a href="payments.md">payments</a></td><td>TODO: waiting until payments tables from QVP and SVP are refactored and posiblyunified into 1 table</td></tr>
<tr><td>6</td><td>last_name</td><td>varchar</td><td></td><td></td><td>Last name as spelled in the certificate document</td></tr>
<tr><td>7</td><td>middle_name</td><td>varchar</td><td></td><td></td><td>Middle name</td></tr>
<tr><td>8</td><td>is_free</td><td>boolean</td><td></td><td></td><td>Free reservation feature. If the reservation was free, then the certificate was free too and it is saved here. TODO: is this field required?</td></tr>
<tr><td>8</td><td>nationality_id</td><td>uuid</td><td></td><td><a href="countries.md">countries</a></td><td>Reference to the country of citizenship (nationality) of the applicant at the time when the certificate was issued</td></tr>
<tr><td>9</td><td>emailed_certificates_count</td><td>integer</td><td></td><td></td><td>When the user clicks 'generate certificate' and the PDF is generated and email job is processed, we increase this field (+1). TODO: is this field required?</td></tr>
<tr><td>9</td><td>passport_number</td><td>varchar</td><td></td><td></td><td>Passport number of a person that the certificate is issued to.</td></tr>
<tr><td>10</td><td>access_token</td><td>varchar</td><td></td><td></td><td>Access token is used a part of URL that is used by the user to download the certificate.</td></tr>
<tr><td>10</td><td>occupation_id</td><td>uuid</td><td></td><td><a href="occupations.md">occupations</a></td><td>Certified occupation</td></tr>
<tr><td>11</td><td>svp_booking_id</td><td></td><td></td><td><a href="svp_bookings.md">svp_bookings</a></td><td>Reference to the initial exam booking</td></tr>
<tr><td>12</td><td>valid_until</td><td>timestamp</td><td></td><td></td><td>Certificate is valid until this timestamp</td></tr>
<tr><td>13</td><td>created_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>14</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>15</td><td>deleted_status</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>