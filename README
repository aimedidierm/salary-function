# Salary Function Assignment 📊

Welcome to the Salary Function Assignment! This project involves working with salary data to perform various tasks related to data processing, error handling, and file handling using Python. Below are the steps I followed to complete the assignment.

## Steps Involved 🛠️

### 1. Import Data 🗄️

- Loaded the salary data into a Jupyter Notebook using pandas.

### 2. Create Employee Function 🧑‍💼

- Developed a Python function that accepts an employee's name as input and returns their details.

### 3. Data Processing with Dictionary 📚

- Processed the salary data using a Python dictionary for easier access.

### 4. Error Handling 🚨

- Implemented error handling to manage cases where employee data might not be found or other potential issues.

### 5. Export Employee Details 📤

- Exported an employee's details to a CSV file and saved it within a zipped folder named "Employee Profile."

### 6. Unzip and Display Data with R 📂

- Used R to unzip and display the data in a user-friendly format.

## Codes explanation

### Import Libraries

```python
import pandas as pd
import os
import zipfile
```

### Import Data

```python
salary_data = pd.read_csv('Total.csv')
```

### Create Employee Function

```python
def get_employee_details(name):
    employee = salary_data[salary_data['EmployeeName'] == name]
    return employee.to_dict(orient='records')
```

### Data Processing with Dictionary

```python
salary_dict = salary_data.set_index('Name').T.to_dict('list')
```

### Error Handling

```python
try:
    # Example of a function call or data processing
    details = get_employee_details('John Doe')
except Exception as e:
    print(f"Error: {e}")
```

### Export Employee Details and Zip File

```python
def export_employee_details(name):
    details = get_employee_details(name)
    df = pd.DataFrame(details)
    file_name = f'{name}_details.csv'
    df.to_csv(file_name, index=False)

    with zipfile.ZipFile('Employee_Profile.zip', 'w') as zipf:
        zipf.write(file_name)
        os.remove(file_name)
```

### R Script (Optional, Add as Text)

```R
# In an R cell or as a text explanation for how to run this in R
unzip("Employee_Profile.zip")
data <- read.csv("Name_details.csv")
print(data)
```

## How to Run the Code 🏃‍♂️

1. Clone the repository or download the files.
2. Open the Jupyter Notebook.
3. Follow the instructions in the notebook to execute the code.

## Requirements 📋

- Python 3.x
- Pandas library
- R (for unzipping and displaying data)

## Contact 💬

If you have any questions, feel free to reach out!

---

Happy Coding! 🎉
