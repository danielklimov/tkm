Tables in QVP Database
=======================

Schema: public

TABLE NAME                                   | DESCRIPTION
---------------------------------------------|--------------------------
[`additional_payment_request`](tables/additional_payment_request.md) | Empty
[`admin_invite`](tables/admin_invite.md) | Invites from one user to another
[`api_key`](tables/api_key.md) | API access permissions
[`application_log`](tables/application_log.md) | App log
[`artistic_merit`](tables/artistic_merit.md) | List of artistic merits
[`bank_account`](tables/bank_account.md) | Bank accounts of TODO: whose accounts?
[`behavioral_competence`](tables/behavioral_competence.md) | Short dict of beh. competences
[`candidate`](tables/candidate.md) | Info about candidates.
[`company_sla_report`](tables/company_sla_report.md) | SLA marks for companies FK companyID
[`discount`](tables/discount.md) | Discount (what for?) FK NationalityID
[`discount_amount`](tables/discount_amount.md) | FK to Discount
[`discount_usage`](tables/discount_usage.md) | empty. FK to Verification Request
[`doctrine_migration_versions`](tables/doctrine_migration_versions.md) | Log of doctrine migrations. TODO: What is a doctrine?
`education_institute` | List of education institutes. I couldn't find the table in PostgreSQL but it exists in Metabase.
`education_institute_additional_fee` | FK to education institutes, FK to education level, FK Major ID. I couldn't find the table in PostgreSQL but it exists in Metabase.
[`education_institute_fee`](tables/education_institute_fee.md) | Empty. FK to: Educ. level, major id, user id
[`education_level`](tables/education_level.md) | Bachelor, Master etc.
[`education_levels_qualifications`](tables/education_levels_qualifications.md) | Link between `education_levels` and `qualification`
[`employee_invite`](tables/employee_invite.md) | Employee invites by Service Providers. FK to service_provider_company
`employment_experience` | Missing from `pg_tables` but exists in Metabase.
[`experience`](tables/experience.md) | Empty. Records about person's employment.
[`fast_track_immediate_record`](tables/fast_track_immediate_record.md) | TODO: clarify
[`fast_track_immediate_request`](tables/fast_track_immediate_request.md) | TODO: what is fast_track_ immediate?
[`fast_track_major_entity_record`](tables/fast_track_major_entity_record.md) | TODO: clarify
[`fast_track_major_entity_request`](tables/fast_track_major_entity_request.md) | TODO: clarify
[`file_storage`](tables/file_storage.md) | Metadata for files used in the system (unique id, user_id, type of file, path etc).
[`invoice`](tables/invoice.md) | Invoices from Takamol to users TODO: clarify.
[`invoice_report`](tables/invoice_report.md) | Additional payment data related to `invoice` - 
[`major`](tables/major.md) | Major (specialization)
[`messages`](tables/messages.md) | Messages of different types between users. TODO: what is context_id
[`messenger_jobs`](tables/messenger_jobs.md) | Jobs that are run by a 'Messenger' that sends messages.
[`notification`](tables/notification.md) | Notifications to users (passport_expired, verification_request, etc.)
[`occupation`](tables/occupation.md) | List of occupations 
[`occupation_category`](tables/occupation_category.md) | Categorization of `occupation`
[`occupations_artistic_merits`](tables/occupations_artistic_merits.md) | Link between `occupation` and `artistic_merits`
[`occupations_behavioral_competences`](tables/occupations_behavioral_competences.md) | Link between `occupation` and `behavioral_competence`
[`occupations_education_levels`](tables/occupations_education_levels.md) | Link between `occupation` and `education_level`
[`occupations_majors`](tables/occupations_majors.md) | Link between `occupation` and `major`
[`one_time_password`](tables/one_time_password.md) | one-time passwords
[`passport`](tables/passport.md) | User passports
[`password_recovery`](tables/password_recovery.md) | password recovery events for `users`
[`qualification`](tables/qualification.md) | Qualifications, i.e. Primary, Bachelor, Master, etc.
[`random_id`](tables/random_id.md) | Some service table with two columns. TODO: clarify.
[`refresh_tokens`](tables/refresh_tokens.md) | Some tokens, generated for user emails valid until some date. TODO: clarify
[`reject_reason`](tables/reject_reason.md) | List of reasons for rejecting a user's verification request.
[`report`](tables/report.md) | Reports from service provider companies.
[`reset_two_factor_key`](tables/reset_two_factor_key.md) | Info on two-factor auth key for a user.
[`security_token`](tables/security_token.md) | Security tokens that have expiration date. TODO: where is it used?
[`service_provider_company`](tables/service_provider_company.md) | Service Providers - companies that issue employee invites. TODO: clarify. FK to bank account.
[`service_provider_company_invoice`](tables/service_provider_company_invoice.md) | Invoices from Takamol to Service Providers. TODO: clarify the term 'Service provider'.
[`service_provider_company_invoice_status`](tables/service_provider_company_invoice_status.md) | Invoice statuses.
[`service_provider_employee`](tables/service_provider_employee.md) | Link between `users` and `service_provider_company`
[`service_provider_employee_report`](tables/service_provider_employee_report.md) | Reports prepared by Takamol for a service provider for a `service_provider_employee`
[`users`](tables/users.md) | Users 
[`verification`](tables/verification.md) | Verification request checkout and payment.
[`verification_payment_transaction`](tables/verification_payment_transaction.md) | Details of verification request payment.
[`verification_payment_transaction_history`](tables/verification_payment_transaction_history.md) | The history of `hyper_pay` responses to hyper_pay payments
[`verification_request`](tables/verification_request.md) | Verification request from user - full information.
[`verification_request_certificate`](tables/verification_request_certificate.md) | Details about verification certificates with references to files.
[`verification_request_education`](tables/verification_request_education.md) | Details about education verifications for a verification request.
[`verification_request_employment`](tables/verification_request_employment.md) | Information about employment history verifications for a verification request.
[`verification_request_nationality`](tables/verification_request_nationality.md) | List of nationalities
[`verification_request_persona`](tables/verification_request_persona.md) | Personal information (name, surname etc.) with FK to `passport`.
[`verification_request_reject_reason`](tables/verification_request_reject_reason.md) | Link between `verification_request` and `reject_reason`
[`verification_request_sla_holds`](tables/verification_request_sla_holds.md) | A 'hold' is a state when a verification request cannot be verified at the moment for certain resons (e.g. educational institution does not respond).
[`verification_request_sla_logs`](tables/verification_request_sla_logs.md) | A log of verification events for a verification request.
[`verification_request_validation`](tables/verification_request_validation.md) | Validations of a verification request (validation is a process that searches for invalid fields in the request).
[`verification_request_validation_history`](tables/verification_request_validation_history.md) | A history of validation attempts for a validation.
