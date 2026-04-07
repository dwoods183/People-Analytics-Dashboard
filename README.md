# People Analytics Dashboard

## Overview
The People Analytics Dashboard is an interactive web-based HR analytics application built with **Python, Dash, Plotly, and Dash Bootstrap Components**. It uses employee-level HR data to help users explore key workforce metrics across departments.

The dashboard is designed to support data-driven decision-making by visualizing trends in:

- Employee turnover
- Average salary by department
- Employee satisfaction
- Department-level diversity by race/ethnicity and gender

This project demonstrates how people analytics can be used to translate HR data into practical business insight.

---

## Features

### 1. Turnover Analysis
Displays the turnover rate for each department using a bar chart.  
This helps identify departments with higher attrition and can support retention-focused decision-making.

### 2. Salary Analysis
Shows the average salary by department.  
This view can be used to compare compensation patterns across teams and identify potential pay structure differences.

### 3. Employee Satisfaction Analysis
Visualizes the average employee satisfaction score by department on a 1–5 scale.  
This provides a quick view of how satisfaction varies across the organization.

### 4. Diversity Analysis
Includes an interactive section that allows the user to switch between:

- **Racial/Ethnic Diversity**
- **Gender Diversity**

The diversity chart is displayed as a stacked bar chart by department, making it easier to compare workforce composition across teams.

---

## Dataset
The dashboard uses the file:

`HRDataset_v14.csv`

### Dataset Summary
- **311 employee records**
- **36 columns**
- Includes employee demographic, compensation, satisfaction, performance, and employment status fields

### Key fields used in this dashboard
- `Department`
- `Termd`
- `Salary`
- `EmpSatisfaction`
- `RaceDesc`
- `Sex`

---

## Metrics Included

### Turnover Rate (%)
Calculated by converting the `Termd` field to numeric format and taking the average by department, then multiplying by 100.

### Average Salary
Calculated as the mean salary for employees in each department.

### Average Employee Satisfaction
Calculated as the mean of the `EmpSatisfaction` score by department.

### Diversity Percentage
Calculated as the percentage distribution of employees within each department by:
- Race/Ethnicity
- Gender

---

## Tech Stack
- **Python**
- **Pandas** for data cleaning and aggregation
- **Plotly Express** for data visualization
- **Dash** for the interactive web application
- **Dash Bootstrap Components** for layout and styling

---

## Project Structure

```bash
People-Analytics-Dashboard/
│
├── People Analytics Dashboard.ipynb   # Main dashboard notebook
├── HRDataset_v14.csv                  # HR dataset used in the dashboard
└── README.md                          # Project documentation
