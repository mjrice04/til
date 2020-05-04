### Comparing lists to find identical values in the same position in list

I ended up needing to find values in two lists that were equivalent and in the same position.The code below did the trick

I was able to use a list comprehension to return a list of values that are in both lists and in the same position.

same_position = `[x for x, y in zip(list_1, list_2) if x == y]`

same_position would return `[2]`
