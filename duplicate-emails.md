https://leetcode.com/problems/duplicate-emails

```MySQL
SELECT email as Email FROM Person GROUP BY email HAVING COUNT(*)>1;
```
