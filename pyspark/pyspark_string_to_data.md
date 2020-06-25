# Pyspark String to date with Select Query

from pyspark.sql.functions import unix_timestamp, from_unixtime

```
df = spark.createDataFrame(
    [("11/25/1991",), ("11/24/1991",), ("11/30/1991",)], 
    ['date_str']
)

df2 = df.select(
    'date_str', 
    from_unixtime(unix_timestamp('date_str', 'MM/dd/yyy')).alias('date')
)

df2.show(truncate=False)
+----------+-------------------+
|date_str  |date               |
+----------+-------------------+
|11/25/1991|1991-11-25 00:00:00|
|11/24/1991|1991-11-24 00:00:00|
|11/30/1991|1991-11-30 00:00:00|
+----------+-------------------+
```
