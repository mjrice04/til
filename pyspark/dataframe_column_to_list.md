# Convert Pyspark DataFrame column to python list

Given a table like below, to make the column **abc** a python list run this command:

```
+---+-----+
|abc|count|
+---+-----+
| 1 |  5  |
| 2 |  9  |
| 3 |  3  |
| 4 |  1  |

`abc_array = [int(row.abc) for row in abc_table.collect()]`
```

This would result in **abc_array** being a python list [1,2,3,4]


