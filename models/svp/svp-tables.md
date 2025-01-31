Tables in SVP Database
=======================

Schema: public

TABLE NAME                                   | DESCRIPTION
---------------------------------------------|--------------------------
[`active_storage_attachments`](tables/active_storage_attachments.md) | Attachments are files attached to records in different database tables, such as legislator and withdrawals. This table links together the record that has an attachment to the table active_storage_blobs that defines the properties of the file itself. Therefore, it is possible to have multiple files attached to one record
[`active_storage_blobs`](tables/active_storage_blobs.md) | List of files stored in active_storage. TODO: what is active_storage?
[`active_storage_variant_records`](tables/active_storage_variant_records.md) | Records attached or connected to active_storage_blobs. TODO: what is that?
[`ar_internal_metadata`](tables/ar_internal_metadata.md) | A dictionary of key-value pairs apparently used to store 
[`assessor_categories`](tables/assessor_categories.md) | Link between assessors and categories (of occupations)
[`assessor_confirmations`](tables/assessor_confirmations.md) | Confirmations of email and phones of assessors. This table is not connected to assessor table
[`assessors`](tables/assessors.md) | List of assessors - persons who conduct assessments of labors. Connected to user table - they are also users
[`categories`](tables/categories.md) | Categorization of occupations
[`categories_test_centers`](tables/categories_test_centers.md) | Link between test_centers and categories - test centers that organize exams for certain categories of occupations
[`certificates`](tables/certificates.md) | Certificate issued to a labor. TODO: specify what do these certificates certify?
[`change_logs`](tables/change_logs.md) | Log of changes of rows in certain (or all?) tables. Table name, old values and new values in json format are stored
[`content_page_items`](tables/content_page_items.md) | Lists of items referencing content_pages.
[`content_pages`](tables/content_pages.md) | List of web pages. TODO: how is this table used?
[`countries`](tables/countries.md) | List of countries
[`country_categories`](tables/country_categories.md) | Link between countries and categories of occupations. TODO: what does it mean if a country is linked to a certain occupation category? Does it mean that skill verification for an occupation that belongs to this category is available only if a labor has the same nationality / citizenship?
[`country_nationalities`](tables/country_nationalities.md) | Link between countries and nationalities. TODO: the meaning of this link? How is it used?
[`credit_balances`](tables/credit_balances.md) | Credit balance for a user
[`exam_constraints`](tables/exam_constraints.md) | Properties of an exam: start time, time limits etc. TODO: This table is not connected to other tables by ref constraints.
[`exam_results`](tables/exam_results.md) | Exam results (score)
[`exam_session_assessors`](tables/exam_session_assessors.md) | Link connecting exam_sessions and assessors.
[`exam_sessions`](tables/exam_sessions.md) | Exam session properties: location, start time etc.
[`flipper_features`](tables/flipper_features.md) | Describes some sort of flow of a web app. TODO: clarify.
[`flipper_gates`](tables/flipper_gates.md) | Describes some sort of logic for web app. TODO: clarify.
[`groups`](tables/groups.md) | Groups of labors assigned to a certain user, a supervisor?
[`invoice_groups`](tables/invoice_groups.md) | Invoice details or invoice 'lines'. One invoice may contain several invoice_groups
[`invoices`](tables/invoices.md) | Invoices from Takamol to legislators and other organizations and persons. TODO: clarify in what way are these invoices connected with skill verification process
[`labor_attaches`](tables/labor_attaches.md) | Link between user_id and country_id. TODO: how is it used?
[`labor_confirmations`](tables/labor_confirmations.md) | Confirmation codes for email and phone confirmations that are sent to labors. The table does not reference labors table, nor any other tables
[`labors`](tables/labors.md) | A labor is a person that is undergoing a skill verification process. Each labor is also a user and has a foreign key referencing user table
[`legislators`](tables/legislators.md) | Organizations that organize skill verification tests/exams
[`nationalities`](tables/nationalities.md) | List of nationalities
[`notifications`](tables/notifications.md) | Notifications to the user in the web app
[`occupations`](tables/occupations.md) | List of occupations
[`passport_recognitions`](tables/passport_recognitions.md) | Results of passport recognition process of the webapp for users and assessors
[`payments`](tables/payments.md) | card payments by users
[`permissions`](tables/permissions.md) | Permissions for certain actions in the app that are granted to certain roles in certain countries
[`prices`](tables/prices.md) | List of prices. Prices are referenced from payments and report_items. TODO: there is no reference to any product or service that specifies what this price is for. Apparently this is a price for 1 verification certificate
[`prometric_answer_logs`](tables/prometric_answer_logs.md) | Answers and scores for questions from prometric_question_logs made by a labor during an exam session
[`prometric_codes`](tables/prometric_codes.md) | Mapping of Prometric codes to categories (of occupations). Prometric is a company that specializes in administering tests
[`prometric_exam_logs`](tables/prometric_exam_logs.md) | Summary info of Prometric exam 'forms' - number of questions, scoring method etc.
[`prometric_exam_result_logs`](tables/prometric_exam_result_logs.md) | Actual results of prometric texams for a reservation
[`prometric_languages`](tables/prometric_languages.md) | List of languages used by Prometric
[`prometric_question_logs`](tables/prometric_question_logs.md) | List of questions for prometric exam with correct answers
[`report_items`](tables/report_items.md) | Cost of verification certificates issued for a group of users. Detail records for reports.
[`reports`](tables/reports.md) | Reports on money spent on verification services. A report is connected to a withdrawal
[`request_logs`](tables/request_logs.md) | Log of web requests to svp-international-api and responses, that include lists of occupations and groups of occupations. TODO: clarify how these requests/responses are used.
[`reservation_credit_payments`](tables/reservation_credit_payments.md) | Links between labors and reservations
[`reservation_credits`](tables/reservation_credits.md) | Links between labors and payments
[`reservation_reschedulings`](tables/reservation_reschedulings.md) | Rescheduled exam_sessions detailed to each particular labor
[`reservations`](tables/reservations.md) | Reservations and resuts of exam_sessions taken by each particular labor, with additional info
[`roles`](tables/roles.md) | Roles - objects used to group permissions for certain actions in the app
[`schema_migrations`](tables/schema_migrations.md) | Some service table for internal use. TODO: clarify
[`shortened_urls`](tables/shortened_urls.md) | URLs of documents (pdfs) mapped to their short unique ids (hashes). TODO: how it is used?
[`temporary_seats`](tables/temporary_seats.md) | Link between labors and exam_sessions - apparently a labor is temporarily attached to an exam session. TODO: how it is used?
[`test_centers`](tables/test_centers.md) | List of test centers owned by legislators
[`test_center_status_requests`](tables/test_center_status_requests.md) | A log of status requests for a test center, if it is active or not. Also includes responses.
[`user_guides`](tables/user_guides.md) | Just a primary key and a creation date. TODO: Are there any objects that reference this table?
[`user_roles`](tables/user_roles.md) | Link between users and roles
[`users`](tables/users.md) | Users: personal info, passwords, some statistics
[`web_service_logs`](tables/web_service_logs.md) | Log of requests and responses to/from web service api calls
[`withdrawals`](tables/withdrawals.md) | Money withdrawals by users. to be spent fo verification exams.

