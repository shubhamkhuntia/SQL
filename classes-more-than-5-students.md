https://leetcode.com/problems/classes-more-than-5-students

```MySQL
select class from courses group by class having count(student)>=5;
```
