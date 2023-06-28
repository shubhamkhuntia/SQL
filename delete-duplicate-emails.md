https://leetcode.com/problems/delete-duplicate-emails/

```MySQL
DELETE p1 FROM Person p1 INNER JOIN Person p2
ON p1.Email = p2.Email where p1.Id > p2.Id
```
