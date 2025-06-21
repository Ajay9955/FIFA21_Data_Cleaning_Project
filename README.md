# FIFA21_Data_Cleaning_Project
Foundational Data Cleaning project of FIFA dataset
# FIFA21 Data Cleaning Project 🧹⚽

This project is part of my Data Engineering learning journey. The goal was to take a raw dataset (`fifa21_raw_data.csv`) and clean it thoroughly using Python and Pandas to produce a high-quality, analysis-ready dataset.

## 📁 Files in This Repository

- `fifa21_raw_data.csv`: Original dataset containing raw information on FIFA 21 players.
- `fifa21_cleaned_data.csv`: Fully cleaned and processed version of the dataset.
- `fifa_cleaning.ipynb`: Jupyter Notebook with detailed step-by-step data cleaning and transformation logic.
- `README.md`: Project summary and documentation.

---

## ✅ Cleaning and Transformation Steps

### 🧹 Column Cleaning
- Removed special characters, extra whitespaces, and standardized column names (lowercase, snake_case).
- Dropped redundant or unused columns (e.g., player photo URLs, profile URLs) and worked with them separately for hands-on practice.

### 🔍 Null Handling
- Detected and analyzed null values across columns.
- Filled `loan_date_end` intelligently by extracting year information from the `team_contract` column.
- Used regex and `.str.extract()` to isolate date values where required.
- Imputed remaining missing values with reasonable constants (e.g., year `2099` for missing end dates).

### 🏷️ Feature Engineering
- Converted and standardized numerical data in text format (`€50M`, `6'1"` height) to numeric forms.
- Ensured correct data types across all fields.

### 🔁 Duplicates
- Checked and removed exact duplicate rows (like row 944 vs row 899).
- Analyzed `name` and `long_name` columns to determine uniqueness and decide whether to drop rows or not.

### 🧪 Data Quality Checks
- Explored column-wise inconsistencies using `value_counts()`, `.dtypes`, and `.describe()`.
- Validated the final cleaned dataset for correctness, structure, and completeness.

---

## 🎯 Key Skills Demonstrated

- Data Cleaning with Pandas
- Regex-Based Extraction
- Null Handling Strategies
- Exploratory Data Analysis
- Data Type Conversions
- Duplicate Detection & Removal
- Feature Engineering & Column Creation

---

