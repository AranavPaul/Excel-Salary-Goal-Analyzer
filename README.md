# 📊 Employee Salary & Goal Analyzer

## 📖 Project Overview
This project is a custom-built Excel application designed to simulate HR salary analysis and employee goal tracking. It utilizes a self-curated dataset of various tech job roles and implements complex logic to validate salary expectations against company standards.

The tool allows users to input their **Experience** and **Salary Expectations**, which are then automatically cross-referenced with the master dataset using logical operators and cell referencing.

## 🧠 Logic & Features Implemented

### 1. Mathematical Operations (Data Processing)
Used basic arithmetic to derive core financial metrics:
- **Total Salary (+)**: Calculated by summing `Annual Salary` and `Bonus`.
- **Bonus Rate (/)**: Derived by dividing `Bonus Max` by `Annual Salary` to understand the variable pay percentage.

### 2. Logical Comparisons (Validation)
Implemented comparison operators to validate data integrity:
- **Salary Verification**: Logic to check `Does Total Salary = Confirmed Salary?`.
- **Bonus Analysis**: Boolean checks for `Is Bonus > Annual Salary?` to flag outliers.

### 3. Cell Referencing & User Goals (Dynamic Analysis)
This is the core interactive feature. A "User Job Goals" table accepts input and uses referencing to compare against the master data:
- **Meets Experience**: Checks if the user's input experience matches the role's requirement.
- **Meets Salary**: Checks if the user's expected salary is within the budget.
- **Meets Both**: A binary (1/0) and Boolean flag indicating if the candidate is a perfect match.

## 📂 Dataset Columns
The master dataset includes the following key attributes:
- **Job Title**: (e.g., Data Scientist, Machine Learning Engineer)
- **Experience (Years)**
- **Annual Salary (INR)**
- **Bonus Max (INR)**
- **Calculated Fields**: Total Salary, Bonus Rate, Confirmation Flags.

## 🚀 How to Use
1. Download the `Main.xlsx` file.
2. Navigate to the **User Goals** sheet (or section).
3. Input your **Years of Experience** and **Expected Salary**.
4. The sheet will automatically update the "Meets Both" column to show if you are eligible for the specific roles listed.

## 🛠 Tools Used
- **Microsoft Excel**: Formulas, Logical Operators (`=`, `>`, `<`), Arithmetic Operators, Cell Referencing.
