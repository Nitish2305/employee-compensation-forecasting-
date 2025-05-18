
# 💼 Employee Compensation Forecasting Application

## Overview

The **Employee Compensation Forecasting Application** is a data-driven tool built using **Python, SQLite, Pandas, and Matplotlib**. It enables HR teams and business managers to:

- Filter employees based on role, location, and status  
- Analyze compensation across roles and experience levels  
- Simulate percentage-based compensation increments  
- Export customized employee datasets as CSV files  

This project is developed in **Google Colab** for ease of collaboration, analysis, and visualization.



## Key Features (User Stories)

###  User Story 1: Filter and Display Active Employees
- Filter employees by **role** and **location**
- View only **active** employees (based on "Active?" or "status")
- Display average compensation by role
- Visualize using a **bar chart**

### User Story 2: Group Employees by Years of Experience
- Categorize employees into experience ranges:
  - `0–1 yrs`, `1–2 yrs`, `2–5 yrs`, `5–10 yrs`, `10–20 yrs`, `20+ yrs`
- Count of employees per range
- Optional: breakdown by **Role** or **Location**
- Visualized using **grouped bar charts**

### User Story 3: Simulate Compensation Increments
- Apply a **global % increment** across all employees
- Apply **custom % increments** per employee or location (optional)
- Show current and updated compensation side by side
- Visualized using a **comparison bar chart**

### User Story 4: Export Filtered Employee Data
- Export filtered data to **CSV**
- Columns included: `Name`, `Role`, `Location`, `Experience`, `Compensation`, `Status`
- Export reflects any **applied increments**


##  Technologies Used

## Technologies Used

| Technology        | Purpose                                  |
|-------------------|-------------------------------------------|
| Python (Pandas)   | Data analysis and transformation          |
| SQLite            | Lightweight relational database           |
| Google Colab      | Cloud-based         Notebook              |
| Matplotlib        | Data visualizations                       |
| Seaborn           | Enhanced plotting visuals                 |
| Streamlit         | Interactive UI dashboard                  |
            



## 🗂 Project Structure
employee-compensation-forecasting
│
├── data
│ └── filtered_employees.csv # Output CSV after filtering/increment
│
├── notebooks
│ └── employee_forecasting.ipynb # Main notebook (Colab-based)
│
├── sql
│ ├── table_creation.sql # Schema for Employees table
│ └── stored_procedures.sql # SQL logic for filtering, grouping
│
├── streamlit_app.py # Optional Streamlit app for UI
│
├── sample_data
│ └── employee_data.csv # Sample employee dataset
│
└── README.md # This file



 data
📄 filtered_employees.csv

This file is the output after applying filters and compensation increments

Automatically generated via the notebook's Export function

notebooks
employee_forecasting.ipynb

This is the  main Jupyter Notebook (Colab)

Contains all logic for:

Loading data

Filtering

Grouping

Increment simulation

CSV export

Visualizations

sql/
table_creation.sql

Script to create the Employees table in SQLite

stored_procedures.sql

Simulated SQL procedures like:

FilterEmployees

CalculateAverageCompensation

GroupByExperience


streamlit_app.py


## How to Run the Application

### Option 1: Run on Google Colab (Recommended - No Setup Required)

1. **Clone or download** this repository.
2. Open the notebook: [`notebooks/employee_forecasting.ipynb`](notebooks/employee_forecasting.ipynb)  
   Or directly open it in [Google Colab](https://colab.research.google.com/)
3. Upload your own dataset (CSV) or use the included sample from `sample_data/employee_data.csv`.
4. Run each cell in order to:
   - Filter employees by role/location/status
   - Group employees by experience levels
   - Simulate compensation increments
   - Export filtered results to CSV
   - Generate visual insights with charts

 No installation or setup required — runs entirely in the browser!


### Option 2: Run Locally with Streamlit (Optional Interactive UI)

Prefer a visual, interactive dashboard? Run it locally with Streamlit:

####  Step-by-Step Setup

1. Make sure **Python 3.7+** is installed
 Install dependencies:

```bash
pip install streamlit pandas matplotlib

streamlit run streamlit_app.py


## For Recruiters & Reviewers

Want to try the app quickly?  
Just open the notebook in Google Colab and run all cells.  
You'll see filtered employee data, grouped insights, compensation forecasts, and downloadable CSV reports — all within 3 minutes.
 steps:
Filter employee records

Analyze experience levels

Simulate increments

Export data

View powerful visual insights


Feel free to reach out via GitHub issues or my profile if you’d like to discuss this project!
