 # Pandas for Data Science 
 ---
 Pandas is a game-changer for data science and analytics, particularly if you came to Python because you were searching for something more powerful than Excel and VBA. Pandas uses fast, flexible, and expressive data structures designed to make working with relational or labeled data both easy and intuitive.
pandas is like Excel in Python: it uses tables (namely DataFrame) and operates transformations on the data. But it can do a lot more.

## Import pandas

 - import pandas as pd

---
### Reading data
- data = pd.read_csv('my_file.csv')

### Writing data
- data.to_csv('my_new_file.csv', index=None)

### Seeing the data
- data.head(3)
### describe()
- df.describe()

### Transposing your data:
- df.T
---
# “stacked”
 DataFrame or Series (having a MultiIndex as the index), the inverse operation of stack() is unstack(), which by default unstacks the last level
---
