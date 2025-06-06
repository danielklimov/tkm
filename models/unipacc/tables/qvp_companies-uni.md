---
title: qvp_companies 
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
<tr><td>1</td><td>id</td><td>uuid</td><td>V</td><td></td><td>autogenerated</td></tr>
<tr><td>2</td><td>name_en</td><td>varchar</td><td></td><td></td><td>Display name in English</td></tr>
<tr><td>3</td><td>name_ar</td><td>varchar</td><td></td><td></td><td>Display name in Arabic</td></tr>
<tr><td>4</td><td>country_id</td><td>uuid</td><td></td><td><a href="countries-uni.md">countries</a></td><td></td></tr>
<tr><td>5</td><td>registration_number</td><td>varchar</td><td></td><td></td><td>Tax (registration) number of the company in the country where it is registered</td></tr>
<tr><td>6</td><td>last_verification_request_assign_date</td><td>timestamp</td><td></td><td></td><td>Statistics: last (the latest) date when a verification request was assigned to this service provider</td></tr>
<tr><td>7</td><td>is_ready</td><td>boolean</td><td></td><td></td><td>TODO: what does 'ready' mean in this context? is_active? Show it in webapp?</td></tr>
<tr><td>8</td><td>legal_name</td><td>varchar</td><td></td><td></td><td>Legal name of the company</td></tr>
<tr><td>9</td><td>kse_license_number</td><td>varchar</td><td></td><td></td><td>A license issued by KSE to the company's own country to perform verification services?</td></tr>
<tr><td>10</td><td>kse_license_issuing_date</td><td>date</td><td></td><td></td><td></td></tr>
<tr><td>11</td><td>kse_license_end_date</td><td>date</td><td></td><td></td><td></td></tr>
<tr><td>12</td><td>email</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>13</td><td>phone_number</td><td>varchar</td><td></td><td></td><td>Phone number without country code</td></tr>
<tr><td>14</td><td>phone_country_code_id</td><td>varchar</td><td></td><td><a href="phone_country_codes-uni.md">phone_country_codes</a></td><td>Country code for phone_number</td></tr>
<tr><td>15</td><td>additional_phone_number</td><td>varchar</td><td></td><td></td><td>Additional telephone number</td></tr>
<tr><td>16</td><td>additional_phone_country_code_id</td><td>varchar</td><td></td><td><a href="phone_country_codes-uni.md">phone_country_codes</a></td><td></td></tr>
<tr><td>17</td><td>website_url</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>18</td><td>building_number</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>19</td><td>street_name</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>20</td><td>neighborhood</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>21</td><td>city</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>22</td><td>postal_code</td><td>varchar</td><td></td><td></td><td></td></tr>
<tr><td>24</td><td>bank_account_holder_name</td><td>varchar</td><td></td><td></td><td>Company name as must be used in payment documents</td></tr>
<tr><td>25</td><td>is_filled</td><td>boolean</td><td></td><td></td><td>TODO: not sure what does that mean but there are records with both true and false, so probably it is still in use</td></tr>
<tr><td>26</td><td>agreed_on_terms_and_conditions</td><td>boolean</td><td></td><td></td><td>The service provider company has agreed on terms and conditions by Takamol</td></tr>
<tr><td>27</td><td>license_document_file_id</td><td>varchar</td><td></td><td><a href="file_storage-uni.md">file_storage</a></td><td>A reference to a file that contains the company's license.</td></tr>
<tr><td>28</td><td>company_status</td><td>varchar</td><td></td><td></td><td>Current status of the company. One of: active, deactivated, suspended.</td></tr>
<tr><td>29</td><td>is_internal</td><td>boolean</td><td></td><td></td><td>There are SPs considered as internal, thus belonging to Takamol holding. They can verify some specific requests, this bool is used to ensure the correct work of the Load balancer</td></tr>
<tr><td>30</td><td>created_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>31</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>32</td><td>deleted_status</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>