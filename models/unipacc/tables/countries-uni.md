---
title: countries 
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
<tr><td>1</td><td>id</td><td>uuid</td><td>V</td><td></td><td>Imitation of uuid created using ISO 3-letter country code. Later on real random uuids may be used.</td></tr>
<tr><td>2</td><td>name_en</td><td>varchar</td><td></td><td></td><td>English name</td></tr>
<tr><td>3</td><td>name_ar</td><td>varchar</td><td></td><td></td><td>Arabic name</td></tr>
<tr><td>4</td><td>nationality_name_en</td><td>varchar</td><td></td><td></td><td>How a person that belongs to this nationality is caled, e.g. Kuwaiti, Peruvian etc. (English)</td></tr>
<tr><td>5</td><td>nationality_name_ar</td><td>varchar</td><td></td><td></td><td>Nationality name in arabic</td></tr>
<tr><td>6</td><td>iso_3_code</td><td>varchar</td><td></td><td></td><td>3-letter ISO code</td></tr>
<tr><td>7</td><td>iso_2_code</td><td>varchar</td><td></td><td></td><td>2-letter ISO code</td></tr>
<tr><td>8</td><td>iso_no</td><td>integer</td><td></td><td></td><td>ISO numeric country code</td></tr>
<tr><td>9</td><td>svp_country_type</td><td>varchar</td><td></td><td></td><td>One of: TARGETED, NON_TARGETED. TARGETED - exams are booked in Takamol test centers. NON_TARGETED - Prometric test centers are used.</td></tr>
<tr><td>10</td><td>svp_test_type</td><td>varchar</td><td></td><td></td><td>Exam type. On of: IN_PERSON, ONLINE. Nullable if svp_country_type = TARGETED</td></tr>
<tr><td>11</td><td>is_mofa_qvp_mandated</td><td>boolean</td><td></td><td></td><td>Qualification verification for citizens (residents?) or this country is mandated (required) by MOFA (Ministry of Foreign Affairs). See also: country_mofa_qvp_mandated_history</td></tr>
<tr><td>12</td><td>is_mofa_svp_mandated</td><td>boolean</td><td></td><td></td><td>Skill verification for citizens (residents?) or this country is mandated (required) by MOFA (Ministry of Foreign Affairs). See also: country_mofa_svp_mandated_history</td></tr>
<tr><td>13</td><td>is_lmh_qvp_mandated</td><td>boolean</td><td></td><td></td><td>Qualification verification for this country is mandated by LMH.</td></tr>
<tr><td>14</td><td>is_lmh_svp_mandated</td><td>boolean</td><td></td><td></td><td>Skill verification for this country is mandated by LMH.</td></tr>
<tr><td>15</td><td>svp_certificate_price</td><td>numeric(18,2)</td><td></td><td></td><td>Price (in USD) for an svp test in this country.</td></tr>
<tr><td>16</td><td>created_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>17</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>18</td><td>deleted_status</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>