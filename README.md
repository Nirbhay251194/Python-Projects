# Student Data Analysis and Classification Dataset

This repository contains a sample dataset for the analysis and classification of online learning students. The dataset includes various attributes related to the students' educational background, demographics, and online learning environment. The dataset can be used for machine learning tasks such as classification, clustering, and predictive analysis.

## Dataset Description

The dataset consists of 1205 records and 11 columns. Each row represents a student, and each column represents an attribute of the student.

### Columns

1. **education_level**: The education level of the student (e.g., School, College, University).
2. **institute_type**: The type of institute the student is enrolled in (e.g., Public, Private).
3. **gender**: The gender of the student (e.g., Male, Female).
4. **age**: The age of the student (integer values ranging from 10 to 30).
5. **device**: The primary device used by the student for online learning (e.g., Desktop, Laptop, Tablet, Smartphone).
6. **it_student**: Whether the student is an IT student (e.g., Yes, No).
7. **location**: The location of the student (e.g., Urban, Rural).
8. **financial_condition**: The financial condition of the student (e.g., Good, Average, Poor).
9. **internet_type**: The type of internet connection used by the student (e.g., Broadband, Mobile Data, Fiber Optic, Satellite).
10. **network_type**: The type of network used by the student (e.g. 4G, 5G).
11. **flexibility_level**: The flexibility level of the student in adapting to online learning (e.g., High, Medium, Low).

## Usage

### Loading the Dataset

You can load the dataset using pandas in Python:

```python
import pandas as pd

# Load the dataset
df = pd.read_csv('student_data.csv')

# Display the first few rows of the dataset
print(df.head())

Example Analysis
Here is an example of how you can perform basic analysis on the dataset:

import pandas as pd

# Load the dataset
df = pd.read_csv('student_data.csv')

# Summary statistics
print(df.describe())

# Distribution of education levels
print(df['education_level'].value_counts())

# Average age of students by education level
print(df.groupby('education_level')['age'].mean())
