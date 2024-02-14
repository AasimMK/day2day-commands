## Get the list of all to tables to delete.

```postgresql
SELECT 'DROP TABLE IF EXISTS ' || tablename || ' CASCADE;' 
FROM pg_tables
WHERE schemaname = 'public'; -- or any other schema
```


## Get column names of a table

```postgresql
SELECT column_name
FROM information_schema.columns
WHERE table_name = '<TABLE_NAME>';
```
