## Get list of all to tables to delete.

SELECT 'drop table if exists ' || tablename || ' cascade;' 
FROM pg_tables
WHERE schemaname = 'public'; -- or any other schema
