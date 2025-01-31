
users
----------------------------


NO | NAME | DATA TYPE | PK | FK | COMMENTS
---|------|-----------|----|----|-------------------
1|`id` | bigint | V |  | 
2|`email` | varchar |  |  | 
3|`reset_password_token` | varchar |  |  | token that was sent via email (?) when user requested to reset his password (forgot password)
4|`reset_password_sent_at` | timestamp |  |  | Time when reset_password_token was sent
5|`remember_created_at` | timestamp |  |  | TODO: time when 'remember me' was set by the user during login?
6|`failed_attempts` | integer |  |  | Count of failed attempts to log in
7|`created_at` | timestamp |  |  | 
8|`updated_at` | timestamp |  |  | 
9|`full_name` | varchar |  |  | Name Surname. TODO: In stg DB there are also records with one word like 'stagelegeightteen'. Does it mean that it can be any username that the user has chosen himself?
10|`country_code` | varchar |  |  | Phone number country code
11|`phone_number` | varchar |  |  | Phone number without country code
12|`otp_required_for_login` | boolean |  |  | One time password required
13|`reset_2fa_token` | varchar |  |  | TODO: clarify
14|`otp_secret_key` | varchar |  |  | One-time password
15|`otp_counter` | integer |  |  | TODO: what does this counter count?
16|`password_digest` | varchar |  |  | bcrypt hash
17|`status` | integer |  |  | values found: 0,1,2. TODO: what do they mean?
18|`last_active_at` | timestamp |  |  | TODO: Does it mean last login time?
19|`rejection_reason` | text |  |  | TODO: Does it mean the user has been rejected to log in, or is it some other kind of rejection?
20|`reset_phone_otp_code` | varchar |  |  | 6-digit code that is sent to user's phone
21|`expiration_token` | timestamp |  |  | TODO: time when password expires?
22|`manager_country_ids` | ARRAY |  |  | 
23|`otp_failed_attempts` | integer |  |  | Count of failed attempts to log in usin one-time passwords
