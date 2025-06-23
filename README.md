# Task_1
using Netflix TV Shows Dataset - Data Cleaning with Python
Data Cleaning Steps
 1. Identify and Handle Missing Values
   - Used `df.isnull().sum()` to detect missing values in each column.
   - Ensured minimal data loss by handling only specific columns with nulls.
 2. Remove Duplicate Rows
   - Checked duplicate entries using `df.duplicated().sum()`
   - Removed exact duplicate rows using `df.drop_duplicates(inplace=True)`
 3. Standardize Text Values
   - Applied `str.strip()` and `str.lower()` to standardize country names.
   - Replaced inconsistent country values (e.g., `'united states'` ➝ `'usa'`).
 4. Convert Date Formats
   - Converted the `date_added` column to proper datetime format using:
 5.Rename colume header
  - Converted the all column as lowercase and without spaces by str.strip().str.lower().str.replace(' ', '_')
 6.check and fix datatype
  - Converted release_year to integer using:
    df['release_year'] = pd.to_numeric(df['release_year'], errors='coerce')
    Ensured date_added is in datetime format.

