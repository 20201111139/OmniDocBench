| UAT   | C++     |
|-------|---------|
| UAT   | Finance |

'an employee fits ajob? if and only if the employee has all skills that are needed by the job.

Please write relational algebra expressions for the following queries.

- 1) Find the name of female employees who have at least one skill needed by the
- 2)

## 2 SQL Query (20 points, 5 points each)

Consider the relational schemas given in problem 1, please write SQL statements to meet the following requests.

- 1)
- Find the jobs that need at least
- 3) Find the names of employees who have the maximum number of skills among all employees.
- 4) Find the employees who fit both the "DEV" and "UAT" jobs.

## 3. Embedded SQL (10 points)

Based on the schemas defined in problem 1 the following embedded SQL program accepts the id of an employee as input and output all skills of the employee. Please fill in the blanks of the program.

main(

EXEC SQL INCLUDE SQLCA;

EXEC SQL BEGIN DECLARE SECTION;

EXEC SQL END DECLARE SECTION;

EXEC SQL CONNECT TO skill\_db USER usel USING passwordl;

cursor CURSOR for

id);

EXEC SQL

for (;

EXEC SQL

if

break;