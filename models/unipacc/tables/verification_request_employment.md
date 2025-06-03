---
title: verification_request_employment 
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
<tr><td>2</td><td>`occupation_id`</td><td>uuid</td><td></td><td>[`occupations`](occupations.md)</td><td>An occupation from the list of occupations that matches occupation_name</td></tr>
<tr><td>3</td><td>`contract_type`</td><td>varchar</td><td></td><td></td><td>Enum: FULL_TIME, PART_TIME</td></tr>
<tr><td>4</td><td>`job_offer_file_id`</td><td>varchar</td><td></td><td>[`file_storage`](file_storage.md)</td><td>Experience or Clearance Certificate </td></tr>
<tr><td>5</td><td>`employment_start_date`</td><td>date</td><td></td><td></td><td>employment start date</td></tr>
<tr><td>6</td><td>`employment_end_date`</td><td>date</td><td></td><td></td><td></td></tr>
<tr><td>7</td><td>`actual_years_count`</td><td>numeric(18,2)</td><td></td><td></td><td>actual working years calculated in accordance with US APPL-38</td></tr>
<tr><td>8</td><td>`employer_name`</td><td>varchar</td><td></td><td></td><td>Employer name</td></tr>
<tr><td>9</td><td>`employer_country_id`</td><td>uuid</td><td></td><td>[`countries`](countries.md)</td><td>Employment address: country</td></tr>
<tr><td>10</td><td>`employer_state_province`</td><td>varchar</td><td></td><td></td><td>Employment address: state/province</td></tr>
<tr><td>11</td><td>`employer_city`</td><td>varchar</td><td></td><td></td><td>Employment address: city</td></tr>
<tr><td>12</td><td>`employer_street`</td><td>varchar</td><td></td><td></td><td>Employment address: street</td></tr>
<tr><td>13</td><td>`employer_building`</td><td>varchar</td><td></td><td></td><td>Employment address: building</td></tr>
<tr><td>14</td><td>`employer_zip_code`</td><td>varchar</td><td></td><td></td><td>Employment address: zip code</td></tr>
<tr><td>15</td><td>`employer_email`</td><td>varchar</td><td></td><td></td><td>Employer's email</td></tr>
<tr><td>16</td><td>`employer_phone_country_code_id`</td><td>uuid</td><td></td><td>[`phone_country_codes`](phone_country_codes.md)</td><td>Employer's phone country code</td></tr>
<tr><td>17</td><td>`employer_phone`</td><td>varchar</td><td></td><td></td><td>Employer's phone number without country code</td></tr>
<tr><td>18</td><td>`employer_website_url`</td><td>varchar</td><td></td><td></td><td>Employer's website</td></tr>
<tr><td>19</td><td>`verification_status`</td><td>varchar</td><td></td><td></td><td>One of: DRAFT, PENDING, IN_PROGRESS, FOR_UPDATE, UPDATED, ON_HOLD, VERIFIED, UNABLE_TO_VERIFY, REJECTED, WITHDRAWN</td></tr>
<tr><td>20</td><td>`sla_days_count`</td><td>integer</td><td></td><td></td><td>Number of days that this vr is in verification - from setting PENDING status to setting one of the final statuses: VERIFIED, UNABLE_TO_VERIFY, REJECTED. This attribute is recalculated daily</td></tr>
<tr><td>21</td><td>`verification_reject_reason_id`</td><td>uuid</td><td></td><td>[`verification_reject_reasons`](verification_reject_reasons.md)</td><td>Nullable. When verification_status is REJECTED or UNABLE_TO_VERIFY, a reject reason is required.</td></tr>
<tr><td>22</td><td>`verification_reject_comment`</td><td>varchar</td><td></td><td></td><td>If verification_reject_reason_id is set and it requires comment, the comment is specified here.</td></tr>
<tr><td>23</td><td>`verification_request_id`</td><td>uuid</td><td></td><td>[`verification_requests`](verification_requests.md)</td><td>VR that this vr_employment is attached to</td></tr>
<tr><td>24</td><td>`qvp_company_id`</td><td>uuid</td><td></td><td>[`qvp_companies`](qvp_companies.md)</td><td>Service provider who does the verification</td></tr>
<tr><td>25</td><td>`qvp_company_employee_id`</td><td>integer</td><td></td><td>[`qvp_company_employees`](qvp_company_employees.md)</td><td>Service provider employee assigned for this verification</td></tr>
<tr><td>26</td><td>`appeal_count`</td><td>integer</td><td></td><td></td><td>Candidate can appeal requests in Rejected or Unable to verify statuses</td></tr>
<tr><td>27</td><td>`first_verification_at`</td><td>timestamp</td><td></td><td></td><td>Same as 'end_verification_at' when verification is done for the first time.</td></tr>
<tr><td>28</td><td>`second_verification_at`</td><td>timestamp</td><td></td><td></td><td>Same as 'end_verification_at' when verification is done for the second time.</td></tr>
<tr><td>29</td><td>`start_verification_at`</td><td>timestamp</td><td></td><td></td><td>Date and time when verification started - verificaton_status became PENDING</td></tr>
<tr><td>30</td><td>`end_verification_at`</td><td>timestamp</td><td></td><td></td><td>Date and time when verification finished - verification_status became one of: VERIFIED, UNABLE_TO_VERIFY, REJECTED, WITHDRAWN</td></tr>
<tr><td>31</td><td>`verifier_user_id`</td><td>uuid</td><td></td><td>[`users`](users.md)</td><td>User that did the verification. This must be the same user as assigned to qvp_company_employee_id</td></tr>
<tr><td>32</td><td>`report_file_id`</td><td>varchar</td><td></td><td>[`file_storage`](file_storage.md)</td><td>uuid. a ref to a file containing the verification report</td></tr>
<tr><td>33</td><td>`created_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>34</td><td>`updated_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>35</td><td>`deleted_status`</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>