---
title: svp_bookings 
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
<tr><td>1</td><td>`id`</td><td>uuid</td><td>V</td><td></td><td>Autoincr</td></tr>
<tr><td>2</td><td>`exam_result`</td><td>varchar</td><td></td><td></td><td>One of: PENDING, PASSED, FAILED</td></tr>
<tr><td>3</td><td>`cbt_exam_status`</td><td>varchar</td><td></td><td></td><td>One of: RESERVED, PENDING, COMPLETED, CANCELED, WITHDRAWN, PAYMENT_FAILED</td></tr>
<tr><td>4</td><td>`certificate_id`</td><td>uuid</td><td></td><td>[`svp_certificates`](svp_certificates.md)</td><td>Skill verification certificate, issued as a result of passing the exam</td></tr>
<tr><td>5</td><td>`applicant_id`</td><td>uuid</td><td></td><td>[`applicants`](applicants.md)</td><td>Applicant that booked an exam session</td></tr>
<tr><td>6</td><td>`exam_session_id`</td><td>uuid</td><td></td><td>[`exam_sessions`](exam_sessions.md)</td><td>An exam session that was booked</td></tr>
<tr><td>7</td><td>`payment_id`</td><td>uuid</td><td></td><td>[`payments`](payments.md)</td><td>TODO: Payment for the exam. Payments for qvp and svp should be united into one table. It's not yet ready</td></tr>
<tr><td>8</td><td>`cancellation_reason`</td><td>varchar</td><td></td><td></td><td>Description why the booking was cancelled. Free text, not an enum.</td></tr>
<tr><td>9</td><td>`is_paid`</td><td>boolean</td><td></td><td></td><td>A flag showing that the booking is paid either with credits or with a card payment</td></tr>
<tr><td>10</td><td>`keycode`</td><td>varchar</td><td></td><td></td><td>Prometric code</td></tr>
<tr><td>11</td><td>`cbt_eligibility_status`</td><td>varchar</td><td></td><td></td><td>When the exam is started, we send the Create Eligibility Request to Prometric, and Prometric returns -1 (failed) or 1 (success) as the response which we store in this column</td></tr>
<tr><td>12</td><td>`practical_eligibility_status`</td><td>varchar</td><td></td><td></td><td>When the exam is started, we send the Create Eligibility Request to Prometric, and Prometric returns -1 (failed) or 1 (success) as the response which we store in this column</td></tr>
<tr><td>13</td><td>`occupation_id`</td><td>uuid</td><td></td><td>[`occupations`](occupations.md)</td><td>The occupation that is going to be verified</td></tr>
<tr><td>14</td><td>`edit_reason`</td><td>varchar</td><td></td><td></td><td>Admins can update the bookings, if they update - the comment is required and stored in this field</td></tr>
<tr><td>15</td><td>`is_hidden`</td><td>boolean</td><td></td><td></td><td>When the reservation is created - it is by default is_hidden: true till payment is made Once User successfully made the payment - change to is_hidden: false In the System only is_hidden: false are shown</td></tr>
<tr><td>16</td><td>`practical_exam_status`</td><td>integer</td><td></td><td></td><td>One of: RESERVED, PENDING, COMPLETED, CANCELED, WITHDRAWN, PAYMENT_FAILED</td></tr>
<tr><td>17</td><td>`access_token`</td><td>varchar</td><td></td><td></td><td>Access token is a part of Reservation Ticket URL to attend the exam (randomly generated)</td></tr>
<tr><td>18</td><td>`cancelled_by_user_id`</td><td>uuid</td><td></td><td>[`users`](users.md)</td><td>The user that cancelled the booking</td></tr>
<tr><td>19</td><td>`cbt_started_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>20</td><td>`cbt_result_received_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>21</td><td>`practical_started_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>22</td><td>`practical_result_received_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>23</td><td>`cbt_prometric_outcome_response`</td><td>text</td><td></td><td></td><td>json</td></tr>
<tr><td>24</td><td>`practical_prometric_outcome_response`</td><td>text</td><td></td><td></td><td>json</td></tr>
<tr><td>25</td><td>`prometric_data`</td><td>text</td><td></td><td></td><td>json.Prometric data (or metadata) about exam</td></tr>
<tr><td>26</td><td>`created_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>27</td><td>`updated_at`</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>28</td><td>`deleted_status`</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>