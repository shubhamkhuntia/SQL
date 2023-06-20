<!-- https://leetcode.com/problems/employees-earning-more-than-their-managers/description/ -->

SELECT a.name as Employee
FROM employee a
INNER JOIN Employee b
ON a.managerId=b.id
where a.salary>b.salary;
