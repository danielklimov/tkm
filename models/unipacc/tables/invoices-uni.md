---
title: invoices 
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
<tr><td>2</td><td>payment_id</td><td>uuid</td><td></td><td><a href="payments-uni.md">payments</a></td><td>Parent payment transaction that this invoice was paid with</td></tr>
<tr><td>3</td><td>file_id</td><td>varchar</td><td></td><td><a href="file_storage-uni.md">file_storage</a></td><td>A reference to the printable copy of the invoice (pdf)</td></tr>
<tr><td>4</td><td>document_number</td><td>varchar(40)</td><td></td><td></td><td>A human-readable invoice number.</td></tr>
<tr><td>5</td><td>currency_code</td><td>varchar</td><td></td><td></td><td>Currency of the amount field (3-letter currency code)</td></tr>
<tr><td>6</td><td>total_amount</td><td>numeric(18,2)</td><td></td><td></td><td>Invoice amount</td></tr>
<tr><td>7</td><td>total_tax_amount</td><td>numeric(18,2)</td><td></td><td></td><td>Total VAT included into 'amount'</td></tr>
<tr><td>8</td><td>buyer_name</td><td>varchar</td><td></td><td></td><td>Name of the buyer (candidate)</td></tr>
<tr><td>9</td><td>qr_code</td><td>text</td><td></td><td></td><td>TODO: what does this QR code contain? How it is encoded?</td></tr>
<tr><td>10</td><td>supplier_tax_id</td><td>varchar</td><td></td><td></td><td>Supplier's (Takamol) tax number.</td></tr>
<tr><td>11</td><td>supplier_name</td><td>varchar</td><td></td><td></td><td>Supplier legal name</td></tr>
<tr><td>12</td><td>supplier_street</td><td>varchar</td><td></td><td></td><td>Supplier address - street name</td></tr>
<tr><td>13</td><td>supplier_location</td><td>varchar</td><td></td><td></td><td>Supplier address - Zipcode and country name</td></tr>
<tr><td>14</td><td>currency_convert_ratio</td><td>numeric(18,4)</td><td></td><td></td><td>TODO: check if it's enough precision. Convertion rate from USD to SAR that is used with this invoice for accounting purposes</td></tr>
<tr><td>15</td><td>zatca_report</td><td>text</td><td></td><td></td><td>ZATCa is a saudi-national e-invoicing system, all invoices are generated through ZATCA. this XML is a klind of a digitally signed elevation file for the invoice. We need to migrate it</td></tr>
<tr><td>16</td><td>created_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>17</td><td>updated_at</td><td>timestamp</td><td></td><td></td><td></td></tr>
<tr><td>18</td><td>deleted_status</td><td>varchar</td><td></td><td></td><td>ACTIVE, DELETED</td></tr>

</table>