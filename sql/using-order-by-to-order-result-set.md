# Using order by to order resultset

There is a keyword called `order by` that can help us order the result set conveniently. For example:

```SQL
SELECT * FROM Orders ORDER BY time_created
```

The default order is ascending and if we want to control the type of order we can use keywords like `DESC`[descending] or `ASC`[ascending].

```SQL
SELECT * FROM Orders ORDER BY time_created DESC
```

[source](http://www.w3school.com.cn/sql/sql_orderby.asp)