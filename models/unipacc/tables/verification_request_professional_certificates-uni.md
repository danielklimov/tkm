---
title: verification_request_professional_certificates 
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
<tr><td>1</td><td>id</td><td>uuid</td><td>V</td><td></td><td>autogen</td></tr>
<tr><td>2</td><td>sla_hold_id</td><td>uuid</td><td></td><td><a href="verification_request_sla_holds-uni.md">verification_request_sla_holds</a></td><td>A ref to the most recent sla hold that was caused by verification of this certificate</td></tr>
<tr><td>3</td><td>professional_certificate_id</td><td>uuid</td><td></td><td><a href="professional_certificates-uni.md">professional_certificates</a></td><td>A reference to the list of known professional certificates</td></tr>
<tr><td>4</td><td>qvp_company_employee_id</td><td>uuid</td><td></td><td><a href="qvp_company_employees-uni.md">qvp_company_employees</a></td><td>SP employee who is assigned for doing the verification</td></tr>
<tr><td>5</td><td>qvp_company_id</td><td>uuid</td><td></td><td><a href="qvp_companies-uni.md">qvp_companies</a></td><td>Service provider who is doing the verification</td></tr>
<tr><td>6</td><td>file_id</td><td>varchar</td><td></td><td><a href="file_storage-uni.md">file_storage</a></td><td>A copy of professional certificate in pdf format</td></tr>
<tr><td>7</td><td>issued_date</td><td>date</td><td></td><td></td><td>Certificate issue date</td></tr>
<tr><td>8</td><td>expiry_date</td><td>date</td><td></td><td></td><td>Certificate expiry date</td></tr>
<tr><td>9</td><td>institute_website</td><td>varchar</td><td></td><td></td><td>Website URL of the institute that issued the certificate</td></tr>
<tr><td>10</td><td>serial_no</td><td>varchar</td><td></td><td></td><td>Human-readable certificate number</td></tr>
<tr><td>11</td><td>verification_status</td><td>varchar</td><td></td><td></td><td>One of: DRAFT, PENDING, IN_PROGRESS, FOR_UPDATE, UPDATED, ON_HOLD, VERIFIED, UNABLE_TO_VERIFY, REJECTED, WITHDRAWN</td></tr>
<tr><td>12</td><td>verification_reject_reason_id</td><td>uuid</td><td></td><td><a href="verification_reject_reasons-uni.md">verification_reject_reasons</a></td><td>Nullable. When verification_status is REJECTED or UNABLE_TO_VERIFY, a reject reason is required.</td></tr>
<tr><td>13</td><td>verification_reject_comment</td><td>varchar</td><td></td><td></td><td>If verification_reject_reason_id is set and it requires comment, the comment is specified here.</td></tr>
<tr><td>14</td><td>verifier_user_id</td><td>varchar</td><td></td><td><a href="users-uni.md">users</a></td><td>User account that was used by the verifier (qvp_company_employee)</td></tr>
<tr><td>15</td><td>appeal_count</td><td>integer</td><td></td><td></td><td>Total number of appeals</td></tr>
<tr><td>16</td><td>first_verification_at</td><td>timestamp</td><td></td><td></td><td>Same as 'end_verification_at' when verification is done for the first time.</td></tr>
<tr><td>17</td><td>second_verification_at</td><td>timestamp</td><td></td><td></td><td>Same as 'end_verification_at' when verification is done for the second time.</td></tr>
<tr><td>18</td><td>start_verification_at</td><td>timestamp</td><td></td><td></td><td>Date and time when verification started - verificaton_status became PENDING</td></tr>
<tr><td>19</td><td>end_verification_at</td><td>timestamp</td><td></td><td></td><td>Date and time when verification finished - verification_status became one of: VERIFIED, UNABLE_TO_VERIFY, REJECTED, WITHDRAWN</td></tr>
<tr><td>20</td><td>sla_days_in_progress</td><td>integer</td><td></td><td></td><td>Statistics: total days in progress</td></tr>
<tr><td>20</td><td>sla_days_count</td><td>integer</td><td></td><td></td><td>Number of days that this vr is in verification - from setting PENDING status to setting one of the final statuses: VERIFIED, UNABLE_TO_VERIFY, REJECTED. This attribute is recalculated daily</td></tr>
<tr><td>21</td><td>sla_days_on_hold</td><td>integer</td><td></td><td></td><td></td></tr>
<tr><td>21</td><td>issuer_name</td><td>varchar</td><td></td><td></td><td>Organization that issued the certificate</td></tr>
<tr><td>22</td><td>report_file_id</td><td>varchar</td><td></td><td><a href="file_storage-uni.md">file_storage</a></td><td>Verification report - printable version in pdf format</td></tr>
<tr><td>23</td><td>validation_id</td><td>uuid</td><td></td><td><a href="verification_request_validations-uni.md">verification_request_validations</a></td><td>A reference to the most recent validation</td></tr>
<tr><td>24</td><td>created_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>25</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>26</td><td>deleted_status</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>