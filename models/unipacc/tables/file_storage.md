file_storage
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | auto-generated
2|`file_type` | varchar |  |  | Enum. One of predefined file types. e.g. VERIFICATION_REQUEST_CERTIFICATE. It defines the table and field that reference this file. TODO: define all possible category codes.
3|`name` | varchar |  |  | Original file name - the name of the file when it was being uploaded. Without path.
4|`size` | integer |  |  | File size in bytes
5|`created_by_user_id` |  |  | [`users`](users.md) | User who created the file
6|`entity_id` | uuid |  |  | References different tables depending on 'file_category_code' field. See file_storage_mappings for details.
7|`file_path` | varchar |  |  | full path to the file on oci bucket  (a.k.a "key" in oci terms)
8|`created_at` | timestamp |  |  | 
9|`updated_at` | timestamp |  |  | 
10|`deleted_status` | varchar |  |  | ACTIVE, DELETED
