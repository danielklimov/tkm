verification_payment_checkout
----------------------------


NO | NAME | DATA TYPE | PK | FK | DESCRIPTION            
---|------|-----------|----|----|-------------
{% sql2md %}
with z as (
select
    t.table_name,
    t.ordinal_position as num,
    t.ordinal_position::varchar as ordinal_position,
    '`' || t.field_name || '`' as field_name,
    case t.data_type
      when 'character varying' then 'varchar'
      when 'timestamp without time zone' then 'timestamp'
      else t.data_type
    end,
    coalesce(t.pk,'') as pk,
    case
      when t.fk = '' then ''
      else '[`' || t.fk || '`](' || t.fk || '.md)'
    end as fk,
    coalesce(t.descr, '') descr,
    coalesce(t.comments1) comments1
  from
    tm_local.stg_uni_column_comments t
  where 1=1
    and t.table_name = 'verification_payment_checkout'
)
select
  z.ordinal_position || '|' || z.field_name || ' | ' || z.data_type || ' | ' || z.pk || ' | ' || z.fk
    || ' | ' || z.descr --|| ' | ' || z.comments1 as md_col
from
  z
order by z.table_name, z.num
{% endsql2md %}

