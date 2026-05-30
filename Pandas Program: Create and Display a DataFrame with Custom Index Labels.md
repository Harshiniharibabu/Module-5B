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
