https://leetcode.com/problems/second-highest-salary

```MySQL
select IFNULL(
(select DISTINCT salary 
from Employee 
ORDER BY salary DESC
LIMIT 1 OFFSET 1), NULL) as SecondHighestSalary;
```
Writing DESC is important cauz sometimes it does ascending order by. Writing distinct is require if there are 2 values with same salary.

```MySQL
select MAX(salary) as SecondHighestSalary from Employee
where salary<(select MAX(salary) from Employee)
```
