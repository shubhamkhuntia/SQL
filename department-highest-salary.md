https://leetcode.com/problems/department-highest-salary/

```MySQL
select Department.name AS Department ,Employee.name AS Employee, Employee.salary
from Employee
LEFT JOIN department
ON employee.departmentId = department.id
WHERE(departmentId, salary) IN
(SELECT departmentId,MAX(salary) FROM Employee GROUP BY departmentId) ;
```

We could have used an inner join too.
