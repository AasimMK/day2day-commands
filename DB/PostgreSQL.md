## Get the list of all to tables to delete.

SELECT 'DROP TABLE IF EXISTS ' || tablename || ' CASCADE;' 
FROM pg_tables
WHERE schemaname = 'public'; -- or any other schema
