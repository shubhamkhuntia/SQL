https://leetcode.com/problems/customers-who-never-order/

```MySQL
select name as "Customers"
from customers
where id not in 
(select customerid from orders);
```
