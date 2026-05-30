# 🧪 Pandas Program: Join Two DataFrames Along Rows

## 🎯 AIM

To write a Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame.

---

## 🧠 ALGORITHM

1. **Import Libraries**: Import the `pandas` library.
2. **Create First DataFrame**: Use a dictionary to create `student_data1`.
3. **Create Second DataFrame**: Use another dictionary to create `student_data2`.
4. **Concatenate DataFrames**: Use `pd.concat()` with `axis=0` to concatenate both DataFrames row-wise.
5. **Display Result**: Print the new combined DataFrame.

---

## 💻 Program

```
import pandas as pd
student_data1 = {
    'StudentID': [1, 2, 3],
    'Name': ['Maya', 'Clara', 'Rita'],
    'Grade': ['A', 'B', 'C']
}
student_data2 = {
    'StudentID': [4, 5, 6],
    'Name': ['Harry', 'Emma', 'Ron'],
    'Grade': ['B', 'A', 'C']
}
df1 = pd.DataFrame(student_data1)
df2 = pd.DataFrame(student_data2)
combined_df = pd.concat([df1, df2], axis=0)
print(combined_df)
```

## Output
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/6845404f-fcbe-4a26-a1ab-4be7a175f0a6" />

## Result
Thus, the program is executed successfully.
