## Flattern List of Python Lists into one List

If you have a list object that is made up of lists you can run the following list comprehension to get one combined list

`flat_list = [item for sublist in my_list for item in sublist]`

Example:

`[['1','2','3'], ['4','5','6']]` becomes `['1','2','3','4','5','6']`

Bonus:

I have a list of strings (my_list) . I want to see which of the items in a larger list (my_large_list) contains any of the strings in my_list

```
column_keeper = []
my_list = ['apple','berry','cherry']
my_large_list = ['apple_sauce', 'tomato', 'potato', 'celery', 'icecream', 'cherry_cola']
for item in my_list:
    sub = item
    sub_list = [s for s in mortgage_columns if sub in s]
    column_keeper.append(sub_list)
flat_list = [item for sublist in column_keeper for item in sublist]
```

Returns `['apple_sauce','cherry_cola']`

 
