
| UAT   | C++     |
|-------|---------|
| UAT   | Finance |

In addition, we define that "an employee fits a job" if and only if the employee has all skills that are needed by the job.

Please write relational algebra expressions for the following queries.

1)
Find the name of female employees who have at least one skill needed by the
"DEV" job.

2)
Find the names of employees who fit the "DEV" job.

## 2. Sql Query (20 Points, 5 Points Each)

Consider the relational schemas given in problem 1, please write SQL statements to meet the following requests.

1)
Find the employees who have not any skills.

2)
Find the jobs that need at least "Java" and "C++" skills.

3)
 Find the names of employees who have the maximum number of skills among all employees.

Find the employees who fit both the "DEV" and "UAT" jobs.

4)

## 3. Embedded Sql (10 Points)

Based on the schemas defined in problem 1, the following embedded SQL program accepts the id of an employee as input , and output all skills of the employee. Please fill in the blanks of the program.

main( )
EXEC SQL INCLUDE SQLCA;
EXEC SQL BEGIN DECLARE SECTION;
char id[10]; char skill [20];
EXEC SQL END DECLARE SECTION;
EXEC SQL CONNECT TO skill_db USER use1 USING password1; 1 EXEC SQL DECLARE skill_cursor CURSOR for _
printf("please input employee id :");
scanf ("%s", id);
2 EXEC SQL _
for (; ;)
{
EXEC SQL _
3 if (
4
) break; printf( "%s\ n", id);

![0_image_0.png](0_image_0.png)

