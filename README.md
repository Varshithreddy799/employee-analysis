# Employee Performance Analysis

## Project Overview
This project analyzes employee performance metrics to identify patterns and insights across different departments, cities, and experience levels. The analysis helps understand how tenure, attendance, and department affiliation impact employee performance scores.

## Dataset Information
The dataset contains **20 employee records** with the following attributes:

| Column | Description | Data Type |
|--------|-------------|-----------|
| employee_id | Unique employee identifier | String |
| name | Employee name (anonymized) | String |
| department | Department (Data, HR, Finance) | String |
| city | Work location (Hyderabad, Bangalore, Mumbai, Delhi) | String |
| join_date | Date of joining | Date |
| review_date | Last performance review date | Date |
| attendance_pct | Attendance percentage (83-97%) | Float |
| performance_score | Performance rating (69-94) | Integer |

## Analysis Performed

### 1. Data Cleaning
- Standardized city and department names (lowercase, trimmed spaces)
- Converted date columns to datetime format
- Handled missing values

### 2. Feature Engineering
- **Tenure Calculation**: Years between join_date and review_date
- **Experience Bands**: 
  - Fresher: < 3 years
  - Medium: 3-7 years  
  - Expert: > 7 years
- **Join Year & Quarter**: Extracted from join_date

### 3. Performance Analysis
- Average performance score by department
- Performance by attendance percentage brackets (0-75%, 75-85%, 85-90%+)
- Performance by tenure duration
- Performance by experience bands
- Performance by city

## How to Run the Analysis

### Prerequisites
```bash
pip install pandas
