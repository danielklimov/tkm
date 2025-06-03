---
title: verification_request_education 
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
<tr><td>2</td><td>`education_level_id`</td><td>uuid</td><td></td><td>[`education_levels`](education_levels.md)</td><td>One of: Diploma, Bachelor, Masters, Doctoral</td></tr>
<tr><td>3</td><td>`education_institute`</td><td>varchar</td><td></td><td></td><td>Name of education institute</td></tr>
<tr><td>4</td><td>`college`</td><td>varchar</td><td></td><td></td><td>Name of the college</td></tr>
<tr><td>5</td><td>`name_record`</td><td>varchar</td><td></td><td></td><td>Aplicant (former student) name as it is written in the educ. certificate</td></tr>
<tr><td>6</td><td>`major_name`</td><td>varchar</td><td></td><td></td><td>Major (specialization)</td></tr>
<tr><td>7</td><td>`start_date_enrollment`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>8</td><td>`end_date_enrollment`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>9</td><td>`institute_street`</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>10</td><td>`institute_building_number`</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>11</td><td>`institute_city`</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>12</td><td>`institute_state`</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>13</td><td>`institute_postal_code`</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>14</td><td>`institute_country`</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>15</td><td>`institute_phone_number`</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>16</td><td>`institute_web_address`</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>17</td><td>`student_id`</td><td>varchar</td><td></td><td></td><td>Institute's internal student id</td></tr>
<tr><td>18</td><td>`student_email`</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>19</td><td>`major_id`</td><td>uuid</td><td></td><td>[`majors`](majors.md)</td><td>A Major from internal list of majors that has been mapped to this edu. cert. </td></tr>
<tr><td>20</td><td>`education_level_status_check`</td><td>varchar</td><td></td><td></td><td>one of: Incompatible, Compatible, Unable to verify</td></tr>
<tr><td>21</td><td>`institute_phone_number_country_code`</td><td>uuid</td><td></td><td>[`phone_country_codes`](phone_country_codes.md)</td><td>Institute phone country code</td></tr>
<tr><td>22</td><td>`verification_status`</td><td>varchar</td><td></td><td></td><td>One of: DRAFT, PENDING, IN_PROGRESS, FOR_UPDATE, UPDATED, ON_HOLD, VERIFIED, UNABLE_TO_VERIFY, REJECTED, WITHDRAWN</td></tr>
<tr><td>23</td><td>`verification_reject_reason_id`</td><td>uuid</td><td></td><td>[`verification_reject_reasons`](verification_reject_reasons.md)</td><td>Nullable. When verification_status is REJECTED or UNABLE_TO_VERIFY, a reject reason is required.</td></tr>
<tr><td>24</td><td>`verification_reject_comment`</td><td>varchar</td><td></td><td></td><td>If verification_reject_reason_id is set and it requires comment, the comment is specified here.</td></tr>
<tr><td>25</td><td>`verification_request_id`</td><td>uuid</td><td></td><td>[`verification_requests`](verification_requests.md)</td><td>TODO: Verification request that this record is connected to. There is a reverse reference - from verification_request to this table. Cardinality - 1:1 Remove this field?</td></tr>
<tr><td>26</td><td>`qvp_company_id`</td><td>uuid</td><td></td><td>[`qvp_companies`](qvp_companies.md)</td><td>The company that is assigned to verify this request</td></tr>
<tr><td>27</td><td>`qvp_company_employee_id`</td><td>uuid</td><td></td><td>[`qvp_company_employees`](qvp_company_employees.md)</td><td>QVP company employee assigned to this request</td></tr>
<tr><td>28</td><td>`appeal_count`</td><td>integer</td><td></td><td></td><td>Count of appeals. An 'appeal' is when the applicant appeals to verify education again after an unsuccessful attempt.</td></tr>
<tr><td>29</td><td>`first_verification_at`</td><td>timestamp</td><td></td><td></td><td>Same as 'end_verification_at' when verification is done for the first time.</td></tr>
<tr><td>30</td><td>`second_verification_at`</td><td>timestamp</td><td></td><td></td><td>Same as 'end_verification_at' when verification is done for the second time.</td></tr>
<tr><td>31</td><td>`start_verification_at`</td><td>timestamp</td><td></td><td></td><td>Date and time when verification started - verificaton_status became PENDING</td></tr>
<tr><td>32</td><td>`end_verification_at`</td><td>timestamp</td><td></td><td></td><td>Date and time when verification finished - verification_status became one of: VERIFIED, UNABLE_TO_VERIFY, REJECTED, WITHDRAWN</td></tr>
<tr><td>33</td><td>`sla_hold`</td><td>uuid</td><td></td><td>[`verification_request_sla_holds`](verification_request_sla_holds.md)</td><td>description of a hold if one exists for this verification</td></tr>
<tr><td>34</td><td>`sla_days_in_progress`</td><td>integer</td><td></td><td></td><td>recalculated and updated every day</td></tr>
<tr><td>34</td><td>`sla_days_count`</td><td>integer</td><td></td><td></td><td>Number of days that this vr is in verification - from setting PENDING status to setting one of the final statuses: VERIFIED, UNABLE_TO_VERIFY, REJECTED, WITHDRAWN. This attribute is recalculated daily</td></tr>
<tr><td>35</td><td>`verifier_user_id`</td><td>uuid</td><td></td><td>[`users`](users.md)</td><td>The user that was doing the verification</td></tr>
<tr><td>35</td><td>`sla_days_on_hold`</td><td>integer</td><td></td><td></td><td>recalculated and updated every day</td></tr>
<tr><td>36</td><td>`education_institute_place_id`</td><td>varchar</td><td></td><td></td><td>Google places Place id if applicable</td></tr>
<tr><td>37</td><td>`education_institute_id`</td><td>varchar</td><td></td><td>[`education_institutes`](education_institutes.md)</td><td>Matching education institute</td></tr>
<tr><td>38</td><td>`report_file_id`</td><td>varchar</td><td></td><td>[`file_storage`](file_storage.md)</td><td>verification report</td></tr>
<tr><td>39</td><td>`validation_id`</td><td>uuid</td><td></td><td>[`verification_request_validations`](verification_request_validations.md)</td><td>Reference to the most recent validation object - details of validation of this request. There can be more than 1 validation per request. This field points to the most recent one.</td></tr>
<tr><td>40</td><td>`exclude_from_already_verified`</td><td>boolean</td><td></td><td></td><td>TODO: does it mean that this request should be excluded from already verified and verified once more? Old field?</td></tr>
<tr><td>41</td><td>`education_certificate_file_id`</td><td>uuid</td><td></td><td>[`file_storage`](file_storage.md)</td><td>Attachment - education certificate</td></tr>
<tr><td>42</td><td>`education_transcript_file_id`</td><td>uuid</td><td></td><td>[`file_storage`](file_storage.md)</td><td>Attachment - transcript</td></tr>
<tr><td>43</td><td>`created_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>44</td><td>`updated_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>45</td><td>`deleted_status`</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>