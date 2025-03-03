
file_storage
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION  | COMMENTS          
---|------|-----------|----|----|--------------|----------
1|`id` | uuid | V |  | auto-generated | 
2|`file_category_code` | varchar |  |  | One of predefined category codes for files. e.g. verification_request_employment. It defines the table and field that reference this file. TODO: define all possible category codes. | 
3|`created_by_user_id` |  |  | [`users`](users.md) | User who created the file | 
4|`entity_id` | uuid |  |  | References different tables depending on 'file_category_code' field. | TODO: There is always a reference from tha table that has an attachment to this table, therefore this field is a reverse reference and technically it is not required. Is it possible to get rid of it?
5|`path` | varchar |  |  | path on oci bucket not including the file name | 
