# Titanic Data Analysis Project:This project explores the famous Titanic dataset using Python. 
It shows how data was cleaned, organized, and visualized to understand which passengers were more
likely to survive the shipwreck.

---

## Tools Used

* **Python**
* **NumPy** (for math operations)
* **Pandas** (for cleaning and managing data)
* **Matplotlib & Seaborn** (for making charts and graphs)

---

## Project Steps

### 1. Data Cleaning
* Checked overall data information using `df.info()` and statistical summary using `df.describe()`.
* Identified missing values using `.isnull().sum()` and checked for duplicate rows.
* Filled missing values in columns:
  * **Age:** Filled missing values with the **median** age.
  * **Embarked:** Filled missing values with the **mode** (most common port).
  * **Deck:** Filled missing values with the word `"Unknown"`.

### 2. Feature Engineering (Creating New Columns)
* Created **`family_size`** by adding family members together.
* Created **`is_alone`** to check if a passenger was traveling alone or with family.
* Created **`age_type`** and **`age_group`** to categorize passengers into different age brackets.

### 3. Data Analysis & Visualizations
* Used **`groupby()`** to compare survival rates across different passenger groups.
* Created the following plots:
  * **Count Plot:** Showed total number of passengers who died vs survived.
  * **Bar Plot:** Compared survival rates between males and females.
  * **Histogram:** Showed age distribution among survivors and non-survivors.
  * **Heatmap:** Showed relationships (correlation) between numerical variables.
  * **Bar Plot:** Compared survival rates across different passenger classes (`pclass`).
  * **Box Plot:** Showed ticket prices (`fare`) paid by different passenger classes (`pclass`).

---

## Project Folder Structure
Data_analysis_titanic/
│
├── notebooks/               # Python code / Jupyter Notebook file
└── README.md                # Project documentation
