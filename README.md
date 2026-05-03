# NumPy_Filter_Array

## Filtering Arrays
Getting some elements out of an existing array and creating a new array out of them is called filtering.

In NumPy, you filter an array using a boolean index list.

If the value at an index is `True` that element is contained in the filtered array, if the value at that index is `False` that element is excluded from the filtered array.

*Creating the Filter Array*
In the example above we hard-coded the `True` and `False` values, but the common use is to create a filter array based on conditions.

`import numpy as np`

`arr = np.array([41, 42, 43, 44])`

`# Create an empty list`
`filter_arr = []`

`# go through each element in arr`
`for element in arr:`
  `# if the element is higher than 42, set the value to True, otherwise False:`
 ` if element > 42:`
   ` filter_arr.append(True)`
  `else:`
  `  filter_arr.append(False)`

`newarr = arr[filter_arr]`

`print(filter_arr)`
print(newarr)

