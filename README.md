# HR Analytics

### Dashboard Link : https://app.powerbi.com/reportEmbed?reportId=873d218e-9c46-4432-9b66-0d0d024e7a92&autoAuth=true&ctid=9b9ae803-fcf8-49a2-995a-557a1a82c2e1



## Problem Statement

The HR Analytics Dashboard provides insights into employee attendance and leave patterns. It enables HR professionals and management to track workforce availability, identify absenteeism trends, and optimize resource planning. The dashboard offers an in-depth analysis of attendance records, leave distribution, department-wise absenteeism, and work-from-home trends.

By leveraging this dashboard, organizations can improve workforce efficiency, address absenteeism concerns, and enhance employee engagement strategies.

### Steps Followed

#### Step 1: Data Loading

- The attendance dataset was imported into Power BI from an Excel file.

- The dataset includes employee codes, names, daily attendance records, and various leave categories.

#### Step 2: Data Cleaning and Transformation

- Opened Power Query Editor to inspect data quality.

- Checked for missing values and inconsistencies.

- Standardized leave codes (P = Present, SL = Sick Leave, WO = Weekly Off, etc.).

- Created calculated columns and DAX measures for in-depth analysis.

#### Step 3: Data Modeling

- Established relationships between employee details and attendance records.

- Optimized data model to improve dashboard performance.

#### Step 4: Report Design

- Applied a professional theme for consistency.

- Implemented slicers to filter by Date, Employee, Department, and Leave Type.

- Designed interactive visuals to enhance user experience.

#### Step 5: Visualizations Used

- KPI Cards:

  Total Employees

  Total Present Days

  Total Leave Days

- Bar Chart:

  Attendance Trends Over Time

  Leave Type Distribution

- Heatmap:

  Monthly Attendance Pattern

- Pie Chart:

  Leave Category Breakdown

- Table Visuals:

  Detailed Attendance Records

- Department-wise Absenteeism Chart:

  Absence rate by department

#### Step 6: DAX Measures

- Total Present Days: 

      Total Present = COUNTROWS(FILTER(Attendance, Attendance[Status] = "P"))

- Total Leave Days: 

      Total Leave = COUNTROWS(FILTER(Attendance, Attendance[Status] <> "P"))

- Attendance Percentage:

      Attendance % = DIVIDE([Total Present], [Total Present] + [Total Leave], 2) * 100

#### Step 7: Publishing the Dashboard

- he report was published to Power BI Service.

- Configured scheduled data refresh for up-to-date insights.

- Shared access with HR and management teams.

### Insights from the Dashboard

#### Attendance Trends

- The overall attendance rate is X%.

- The highest absenteeism was recorded in Month Y.

#### Leave Distribution

- Sick Leave accounts for X% of total leaves.

- Work-from-home trend increased by Y% compared to the previous month.

#### Department-wise Analysis

- Department A has the highest absenteeism rate of Z%.

- Department B maintains the highest attendance consistency.

#### Employee Engagement Insights

- X% of employees have an attendance rate above Y%.

- Z% of employees took more than N leaves in the past three months.

### Conclusion

The HR Analytics Dashboard enables organizations to monitor employee attendance patterns and take proactive measures to improve workforce productivity. By analyzing attendance trends and absenteeism patterns, HR teams can enhance policies and support employee well-being.

### Future Improvements

- Integration with payroll systems for automated leave tracking.

- Predictive modeling for absenteeism trends.

- Employee satisfaction surveys linked to attendance insights.
