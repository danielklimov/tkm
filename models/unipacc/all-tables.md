Tables in Uni PACC Database
============================


TABLE NAME                                   | DESCRIPTION
---------------------------------------------|--------------------------
{% sql2md %}
select
  '[`' || t.table_name || '`](tables/' || t.table_name || '.md) | ' || t.comments1 as md_line
  --t.*
from
  tm_local.stg_uni_table_comments t
order by
  t.table_name
{% endsql2md %}
