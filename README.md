This code downloads files from AWS, with the use of pandas dataframes merges the data and then uploads to Postgre Database. 

Ran into error with psycopg2-binary build so was unable to successfully load data into Database but the last cell
code should have capability to upload data to DB with environments that have psycopg2 properly installed. Within the comments 
of the second to last cell have included the SQL query that would be used in postgre to return receiver total yards along with the 
equivalent logic in pandas to display what results would be.
SQL QUERY:
# SELECT 
#   SUM(Chase_Yards), 
#   SUM(Boyd_Yards),
#   SUM(Higgins_Yards), 
#   CONCAT(SUM(CASE WHEN Result = 'W' THEN 1 ELSE 0 END),
#           '-',
#            CASE WHEN Result = 'L' THEN 1 ELSE 0 END)) AS Record
# FROM devon_adjei
