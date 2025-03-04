Tables in Uni PACC Database
============================


TABLE NAME                                   | DESCRIPTION
---------------------------------------------|--------------------------
[`applicants`](tables/applicants.md) | Applicants - both QVP and SVP
[`applicants_passport_history`](tables/applicants_passport_history.md) | History of changes of applicant's current passport.
[`assessor_occupation_categories`](tables/assessor_occupation_categories.md) | Occupation categories that can be assessed by an assessor.
[`assessors`](tables/assessors.md) | Assessors - persons who supervise skill verification process for SVP applicants
[`countries`](tables/countries.md) | List of countries
[`country_qvp_statuses`](tables/country_qvp_statuses.md) | Countries for which QVP verification is required for all occupations.
[`education_institutes`](tables/education_institutes.md) | List of education institutes
[`education_institutes_additional_fees`](tables/education_institutes_additional_fees.md) | Some Universities charge for verifying the Applicants info. Here we collect the info about these fees
[`education_levels`](tables/education_levels.md) | Bachelor, Master etc.
[`fast_track_immediate_records`](tables/fast_track_immediate_records.md) | Fast track is a special flag created to highlight the need to verify specific applicant as soon as possible.
[`file_storage`](tables/file_storage.md) | Metadata for files used in the system as attachments to records in other tables.
[`majors`](tables/majors.md) | Majors (specializations)
[`occupation_categories`](tables/occupation_categories.md) | Categorization of occupations - unified QVP and SVP categories
[`occupations`](tables/occupations.md) | List of occupations, unified QVP and SVP occupation lists
[`occupation_subcategories`](tables/occupation_subcategories.md) | Additional categorization of occupations
[`passports`](tables/passports.md) | 
[`phone_country_codes`](tables/phone_country_codes.md) | International phone country codes
[`qvp_companies`](tables/qvp_companies.md) | Service providers for qualification verification
[`qvp_company_bank_accounts`](tables/qvp_company_bank_accounts.md) | Bank accounts owned by service provider companies
[`qvp_company_employee_reports`](tables/qvp_company_employee_reports.md) | QVP reports made by QVP company employees
[`qvp_company_employees`](tables/qvp_company_employees.md) | A link between users and qvp_companies - a user that logs into PACC on behalf of a QVP company.
[`qvp_company_invoices`](tables/qvp_company_invoices.md) | Invoices from QVP service providers to Takamol
[`qvp_company_invoice_status_history`](tables/qvp_company_invoice_status_history.md) | History of changes of qvp_company_invoices.invoice_status field
[`qvp_company_reports`](tables/qvp_company_reports.md) | Reports made by QVP service providers as part of invoicing process
[`similar_occupations`](tables/similar_occupations.md) | Occupations similar to the one specified in a job offer that can also be used for verification and calculation of eligibility score
[`users`](tables/users.md) | user accounts information
[`verification_payment_checkout`](tables/verification_payment_checkout.md) | Verification request checkout and payment.
[`verification_reject_reasons`](tables/verification_reject_reasons.md) | List of possible reasons for rejecting a verification request.
[`verification_request_certificates`](tables/verification_request_certificates.md) | Certificates that represent results of processing verification requests
[`verification_request_education`](tables/verification_request_education.md) | Details about education verifications for a verification request.
[`verification_request_eligibility_scores`](tables/verification_request_eligibility_scores.md) | Eligibility scores for a VR
[`verification_request_employment`](tables/verification_request_employment.md) | Information about employment history verifications for a verification request.
[`verification_request_personas`](tables/verification_request_personas.md) | Personal information for a verification_request (name, surname etc.). An extension of verification_requests table
[`verification_request_professional_certificates`](tables/verification_request_professional_certificates.md) | Applicants' professional certificates that must be verified as part of VR
[`verification_request_reject_reasons`](tables/verification_request_reject_reasons.md) | Reasons why a particular verification request was rejected
[`verification_requests`](tables/verification_requests.md) | Qualification verification request from an applicant - the central table that stores basic info. Tables that contain other pieces of information on verification request reference this table. 
[`verification_request_sla_holds`](tables/verification_request_sla_holds.md) | A 'hold' is a state when a verification request cannot be verified at the moment for certain resons (e.g. educational institution does not respond).
[`verification_request_validations`](tables/verification_request_validations.md) | Validations of verification request with history
[`verification_request_verified_employment_experience`](tables/verification_request_verified_employment_experience.md) | A link between vr_employment and vr that signifies that vr_employment has been verified