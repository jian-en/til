# Aggregate results from sql

Sometimes we use sql to generate results and want to do some calculations on the results. Obviously we can union the results by the keyword `union`:

```sql
SELECT product_price FROM Product
UNION
SELECT product_price FROM Customer;
```

The statement above union the result and automatically distinct the results and we can use `UNION ALL` to keep all the results. Furthermore if we want to do some caculation on the sql result, go ahead using the nested sql statements:

```sql
SELECT (SELECT sum(a.product_price) FROM Product a)
/
(SELECT count(distinct(user_id)) FROM Customer b);
```

You may notice `TABLE alias`. It is convenient to avoid the conflict of table names.

[source](http://www.w3schools.com/sql/sql_union.asp)