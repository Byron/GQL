An aggregate function in GQL performs a calculation on multiple values and returns a single value

### Aggregation `max`
Accept field name with `NUMBER` to calculate the maximum value of it for all elements until the current one

```sql
SELECT name, commit_count, max(commit_count) FROM branches
```

### Aggregation `count`
The function COUNT() is an aggregate function that returns the number of items in a group

```sql
SELECT name, max(name) FROM commits GROUP BY name
```