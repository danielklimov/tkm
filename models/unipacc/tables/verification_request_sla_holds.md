verification_request_sla_holds
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION  | COMMENTS          
---|------|-----------|----|----|--------------|----------
1|`id` | uuid | V |  | autogen
2|`request_id` | uuid |  | [`verification_requests`](verification_requests.md) | VR that caused this hold
3|`education_id` | uuid |  | [`verification_request_education`](verification_request_education.md) | Education record that caused a hold
4|`profeccional_certificate_id` | uuid |  | [`verification_request_professional_certificates`](verification_request_professional_certificates.md) | Professional certificate record that caused a hold
5|`employment_experience_id` | uuid |  | [`verification_request_employment`](verification_request_employment.md) | Employment record that caused a hold
6|`user_id` | uuid |  | [`users`](users.md) | User that created a hold
7|`start_ts` | long |  |  | unix epoch (ms since 1 jan 1970)
8|`stop_ts` | long |  |  | unix epoch (ms since 1 jan 1970)
9|`hold_duration_secs` | long |  |  | Hold duration in seconds
10|`hold_status` | varchar |  |  | one of: on_hold, in_progress
11|`reason` | varchar |  |  | Arbitrary string e.g. 'Educational institute does not respond'
12|`description` | text |  |  | Detailed description of the hold
13|`revoke_comment` | varchar |  |  | Arbitrary string - a description of how/why the hold was revoked
14|`previous_status` | varchar |  |  | Previous status of verification_request, that is, the status of VR at the moment when the hold was created
15|`created_at` | timestamp |  |  | 
16|`updated_at` | timestamp |  |  | 
17|`deleted_status` | integer |  |  | 0 - active record, 1 - deleted record.
