# Book Data - My First DataFrame

This is my very first mini data project using Python and pandas.

## What I’ve done so far:

- Created a Python dictionary with book information (title, author, year, price, etc.)
- Converted that dictionary into a pandas DataFrame (table)
- Displayed the table in the console

## Tools used:
- Python 
- pandas 
- Thonny (IDE)

## Next steps:
- Learn how to filter and analyze the data
- Practice basic data manipulations (sorting, conditions)
- Add comments and keep improving the script

---

### 🐍 My Python Code

```python
# Step 1: Import libraries
import pandas as pd
from datetime import datetime

# Step 2: Create a dictionary with book data
books_data = {
    'id': [1, 2, 3, 4, 5],
    'book_title': ['1984', 'Lord of the Flies', 'To Kill a Mockingbird', 'Wuthering Heights', 'Trainspotting'],
    'author_name': ['George Orwell', 'William Golding', 'Harper Lee', 'Emily Brontë', 'Irvine Welsh'],
    'publication_year': [1949, 1954, 1960, 1847, 1993],
    'number_of_pages': [328, 224, 281, 416, 344],
    'book_genre': ['Dystopia', 'Fiction', 'Fiction', 'Fiction', 'Fiction'],
    'book_price': [9.99, 11.59, 8.75, 9.27, 11.13],
    'date_added': [
        datetime(2023, 10, 1),
        datetime(2023, 10, 3),
        datetime(2023, 10, 5),
        datetime(2023, 10, 7),
        datetime(2023, 10, 9)
    ]
}

# Step 3: Convert dictionary to DataFrame
books_df = pd.DataFrame(books_data)

# Step 4: Display the DataFrame
print(books_df)
