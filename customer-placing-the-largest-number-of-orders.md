https://leetcode.com/problems/customer-placing-the-largest-number-of-orders

```MySQL
select customer_number from orders GROUP BY customer_number ORDER BY count(order_number) desc limit 1;
```
