svp_test_center_occupation_categories
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
1|`id` | uuid | V |  | autoincr
2|`test_center_id` | uuid |  | [`svp_test_centers`](svp_test_centers.md) | Test center
3|`occupation_category_id` | uuid |  | [`occupation_categories`](occupation_categories.md) | Occupation category
4|`created_at` | timestamp |  |  | 
5|`updated_at` | timestamp |  |  | 
6|`deleted_status` | varchar |  |  | ACTIVE, DELETED
