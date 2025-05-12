Tables in Uni PACC Database
============================


TABLE NAME                                   | DESCRIPTION
---------------------------------------------|--------------------------
[`admin_invite`](tables/admin_invite.md) | 
[`applicant_order_items`](tables/applicant_order_items.md) | 
[`applicant_orders`](tables/applicant_orders.md) | 
[`applicant_passport_history`](tables/applicant_passport_history.md) | 
[`applicants`](tables/applicants.md) | TODO missing mappings!
[`application_log`](tables/application_log.md) | 
[`assessor_cities`](tables/assessor_cities.md) | 
[`assessor_intl_qualifications`](tables/assessor_intl_qualifications.md) | 
[`assessor_languages`](tables/assessor_languages.md) | 
[`assessor_occupation_categories`](tables/assessor_occupation_categories.md) | 
[`assessors`](tables/assessors.md) | TODO: international_qualifications - array, move to a separate table
[`countries`](tables/countries.md) | TODO: check source mappings. see fields
[`country_mofa_qvp_mandated_history`](tables/country_mofa_qvp_mandated_history.md) | 
[`country_mofa_svp_mandated_history`](tables/country_mofa_svp_mandated_history.md) | 
[`country_qvp_statuses`](tables/country_qvp_statuses.md) | TODO: DK: Is is the same as is_mofa_mandated flag for a country that is stored in countries table?
[`draft_verification_request_eligibility_scores`](tables/draft_verification_request_eligibility_scores.md) | 
[`education_institutes`](tables/education_institutes.md) | 
[`education_institutes_additional_fees`](tables/education_institutes_additional_fees.md) | 
[`education_levels`](tables/education_levels.md) | 
[`employee_invites`](tables/employee_invites.md) | 
[`employee_invite_verification_types`](tables/employee_invite_verification_types.md) | 
[`exam_results`](tables/exam_results.md) | 
[`exam_session_assessors`](tables/exam_session_assessors.md) | 
[`exam_sessions`](tables/exam_sessions.md) | 
[`fast_track_immediate_records`](tables/fast_track_immediate_records.md) | 
[`fast_track_immediate_request_docs`](tables/fast_track_immediate_request_docs.md) | 
[`fast_track_immediate_requests`](tables/fast_track_immediate_requests.md) | 
[`fast_track_major_entity_records`](tables/fast_track_major_entity_records.md) | 
[`fast_track_major_entity_request_docs`](tables/fast_track_major_entity_request_docs.md) | 
[`fast_track_major_entity_requests`](tables/fast_track_major_entity_requests.md) | 
[`file_storage`](tables/file_storage.md) | 
[`general_application_settings`](tables/general_application_settings.md) | 
[`invoice_items`](tables/invoice_items.md) | 
[`invoice_reports`](tables/invoice_reports.md) | TODO: include into payment?
[`invoices`](tables/invoices.md) | 
[`legislators`](tables/legislators.md) | TODO: see is_active field
[`majors`](tables/majors.md) | 
[`occupation_categories`](tables/occupation_categories.md) | 
[`occupation_edication_levels`](tables/occupation_edication_levels.md) | 
[`occupation_majors`](tables/occupation_majors.md) | 
[`occupation_nationalities_mandated_in`](tables/occupation_nationalities_mandated_in.md) | 
[`occupation_relevant_professional_certificates`](tables/occupation_relevant_professional_certificates.md) | 
[`occupations`](tables/occupations.md) | 
[`occupation_subcategories`](tables/occupation_subcategories.md) | 
[`passports`](tables/passports.md) | 
[`payments`](tables/payments.md) | 
[`phone_country_codes`](tables/phone_country_codes.md) | TODO: is there any source table that can be used to fill it up?
[`professional_certificates`](tables/professional_certificates.md) | 
[`prometric_answer_logs`](tables/prometric_answer_logs.md) | 
[`prometric_codes`](tables/prometric_codes.md) | 
[`prometric_exam_logs`](tables/prometric_exam_logs.md) | TODO: see comments for fields
[`prometric_languages`](tables/prometric_languages.md) | 
[`prometric_question_logs`](tables/prometric_question_logs.md) | 
[`qvp_certificates`](tables/qvp_certificates.md) | 
[`qvp_companies`](tables/qvp_companies.md) | 
[`qvp_company_bank_accounts`](tables/qvp_company_bank_accounts.md) | 
[`qvp_company_employee_reports`](tables/qvp_company_employee_reports.md) | TODO: Unsure, which tables are referenced in it. See fields
[`qvp_company_employees`](tables/qvp_company_employees.md) | 
[`qvp_company_invoices`](tables/qvp_company_invoices.md) | 
[`qvp_company_invoice_status_history`](tables/qvp_company_invoice_status_history.md) | 
[`qvp_company_reports`](tables/qvp_company_reports.md) | 
[`qvp_company_sla_reports`](tables/qvp_company_sla_reports.md) | 
[`qvp_company_verification_types`](tables/qvp_company_verification_types.md) | 
[`random_numbers`](tables/random_numbers.md) | 
[`similar_occupations`](tables/similar_occupations.md) | 
[`svp_bookings`](tables/svp_bookings.md) | 
[`svp_certificates`](tables/svp_certificates.md) | TODO: certificate pdf is not saved to file_storage, but is generated anew each time the user clicks 'generate'. Is it ok or is it better to generate it once and then store the generated pdf it in oci? See also comments to 1 field
[`svp_country_nationalities`](tables/svp_country_nationalities.md) | 
[`svp_country_occupation_categories`](tables/svp_country_occupation_categories.md) | 
[`svp_exam_session_temp_seats`](tables/svp_exam_session_temp_seats.md) | 
[`svp_test_center_occupation_categories`](tables/svp_test_center_occupation_categories.md) | 
[`svp_test_centers`](tables/svp_test_centers.md) | 
[`users`](tables/users.md) | 
[`verification_payment_checkout`](tables/verification_payment_checkout.md) | TODO: see payment_type field. To clarify.
[`verification_payment_transaction_history`](tables/verification_payment_transaction_history.md) | 
[`verification_payment_transactions`](tables/verification_payment_transactions.md) | 
[`verification_reject_reasons`](tables/verification_reject_reasons.md) | 
[`verification_request_education`](tables/verification_request_education.md) | TODO: there are some circular references. One table references another and another table references this table back. See fields. Decide what to do with them - either leave them be or delete one of the references.
[`verification_request_education_verification_history`](tables/verification_request_education_verification_history.md) | 
[`verification_request_eligibility_scores`](tables/verification_request_eligibility_scores.md) | 
[`verification_request_employment`](tables/verification_request_employment.md) | TODO: see contract_type_id field. See also verification_reject_reason - migration logic.
[`verification_request_personas`](tables/verification_request_personas.md) | 
[`verification_request_professional_certificates`](tables/verification_request_professional_certificates.md) | TODO: see migration details for columns reject_reason_id
[`verification_request_progress_status`](tables/verification_request_progress_status.md) | 
[`verification_request_reject_reasons`](tables/verification_request_reject_reasons.md) | 
[`verification_requests`](tables/verification_requests.md) | 
[`verification_request_sla_holds`](tables/verification_request_sla_holds.md) | The table has been merged into verification_request_sla_logs
[`verification_request_sla_log`](tables/verification_request_sla_log.md) | 
[`verification_request_validations`](tables/verification_request_validations.md) | 
[`verification_request_verification_types`](tables/verification_request_verification_types.md) | 
[`verification_services`](tables/verification_services.md) | 
[`vr_verified_employment`](tables/vr_verified_employment.md) | 