# NumPy Program: Column-wise Sorting of a 2D Array

## 🎯 Aim
To write a **NumPy** program that sorts the elements in each column of a given 2D array in ascending order.

## 🧠 Algorithm

1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Accept a 2D NumPy array from the user.
3. **Sort Column-wise**: Use the `np.sort()` function with `axis=0` to sort each column in ascending order.
4. **Store Result**: Store the sorted result in a new array.
5. **Display Output**: Print the original array and the column-wise sorted array.

## 🧾 Program
```
import numpy as np
array = np.array([[7, 67, 87],
                [43, 54, 98],
                [78, 8, 9]])
sorted_array = np.sort(array, axis=0)
print("Original array:\n", array)
print("Column-wise sorted array:\n", sorted_array)
```

## Output
<img width="1913" height="1016" alt="image" src="https://github.com/user-attachments/assets/e05bd80b-90fd-438b-8371-2f0efd887a60" />

## Result
Thus, the program is executed successfully.

# # NumPy Program: Find Indices Where Elements in Array x are Greater Than or Equal to Corresponding Elements in Array y

## 🎯 Aim
To write a Python program using **NumPy** that finds the indices where elements in array `x` are greater than or equal to their corresponding elements in array `y`.

## 🧠 Algorithm
1. **Import NumPy**: Import the NumPy library.
2. **Define Arrays**: Define two NumPy arrays, `x` and `y`, with the same shape (i.e., same number of elements).
3. **Use Boolean Indexing**: 
   - `x > y` gives a boolean array where elements of `x` are greater than `y`.
   - `x == y` gives a boolean array where elements of `x` are equal to `y`.
4. **Find Indices**: Use `np.where()` to get the indices where the conditions `x >= y` are satisfied.
5. **Print Indices**: Print the indices where the condition holds true.

## 🧾 Program

```
import numpy as np
x = np.array([1, 30, 54, 70, 22])
y = np.array([2, 7, 80, 11, 45])
indices = np.where(x >= y)
print("Indices where x >= y:", indices[0])
```

## Output
<img width="1919" height="1020" alt="image" src="https://github.com/user-attachments/assets/27b60fe8-ac88-4db6-8938-d6ace1176ef7" />

## Result
Thus, the program is executed successfully.

# NumPy Program: Replace the Second Column in a 2D Array

## 🎯 Aim
To write a **NumPy** program that deletes the second column from a given 2D array and inserts a new column at the same position.

## 🧠 Algorithm
1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Get a 2D NumPy array and a new column (as another array) from the user.
3. **Delete Column**: Use `np.delete()` to remove the second column (index 1) from the original array.
4. **Insert Column**: Use `np.insert()` to insert the new column at the second column's original position.
5. **Display Result**: Print the updated array with the replaced column.

## 🧾 Program

```
import numpy as np
a = np.array([[1, 2, 3],
                [4, 5, 6],
                [7, 8, 9]])
new_col = np.array([10, 11, 12])
a = np.delete(a, 1, axis=1)
a = np.insert(a, 1, new_col, axis=1)
print("Updated array:\n", a)
```

## Output
<img width="1919" height="1023" alt="image" src="https://github.com/user-attachments/assets/d3f9477f-6118-441c-ac5f-3089752b8335" />

## Result
Thus, the program is executed successfully.

# Pandas Program: Create and Display a DataFrame with Custom Index Labels

## 🎯 Aim

To create and display a **DataFrame** using the **Pandas** library in Python from a given dictionary, and apply specific index labels to the rows.

---

## 🧠 Algorithm

1. **Import Libraries**: Import the required libraries – `pandas` and `numpy`.
2. **Create Dictionary**: Define a dictionary `exam_data` with keys: `'name'`, `'score'`, `'attempts'`, and `'qualify'`.
3. **Index Labels**: Create a list of custom index labels called `labels`.
4. **Create DataFrame**: Use `pd.DataFrame()` to create the DataFrame by passing the dictionary and index labels.
5. **Display Output**: Display the DataFrame using `print()` or by simply calling the DataFrame variable.

---

## 💻 Program
```
import pandas as pd
import numpy as np
exam_data = {
    'name': ['Anthony', 'Diana', 'Kate', 'Jake', 'Emma', 'Matthew', 'Diya', 'Tara', 'Riya'],
    'score': [23.6,45.1,34,23.2,43,54.6,23,23.5,12.0],
    'attempts': [1, 3, 2, 3, 2, 3, 1, 1, 2],
    'qualify': ['yes', 'no', 'yes', 'no', 'no', 'yes', 'yes', 'yes', 'no']
}
labels = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i']
df = pd.DataFrame(exam_data, index=labels)
print(df)
```

## Output
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/753b4dd9-3e17-4013-a42c-e494d35bde61" />

## Result
Thus, the program is executed successfully.
