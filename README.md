
Context

I need to develop a professional KPI Dashboard for Airport Ground Support Equipment (GSE) operations. Users will upload monthly Excel files containing operational KPI data. The dashboard must automatically read all sheets, calculate KPIs, and display management-level insights.

Role

Act as a Senior Project Manager, Airport Operations Consultant, BI Dashboard Architect, UI/UX Expert, and Full-Stack Developer.

Objective

Design and generate a production-ready HTML dashboard that allows users to upload monthly Excel files and automatically generate KPI reports, trends, charts, analytics, and operational insights.

Business Background

The uploaded Excel files contain multiple worksheets such as:

1. GPU Uptime
2. GPU Serviceability & Availability
3. PCA Uptime
4. PCA Serviceability & Availability
5. PBB Serviceability & Availability
6. Airline Complaints
7. Major Complaints / Breakdown
8. Removed Item Inventory
9. PBB Breakdown Reports
10. Usage Summary
11. Kaizen / Improvement Activities
12. Operator Performance Report

The dashboard should automatically identify worksheets and populate relevant sections. 【1-2d1382】

Functional Requirements

### 1. File Upload Module

- Support .xlsx and .xls formats.
- Drag-and-drop upload area.
- File validation.
- Loading indicator.
- Display uploaded file name and upload timestamp.
- Support future uploads having same sheet structure.

### 2. Executive KPI Dashboard

Display top KPI cards:

- Total GPU Units
- Total PCA Units
- Total PBB Units
- GPU Availability %
- GPU Serviceability %
- PCA Availability %
- PCA Serviceability %
- PBB Availability %
- PBB Serviceability %
- Total Complaints
- Major Breakdowns
- Total Flights Handled
- Equipment Usage %
- Equipment Non-Usage %
- Kaizen Improvements Implemented

### 3. Operations Dashboard

Create charts for:

A. GPU Monitoring
- Daily Uptime Trend
- Stand-wise Uptime
- Top 10 Lowest Uptime Units
- Serviceability Trend
- Availability Trend

B. PCA Monitoring
- Daily Uptime Trend
- Serviceability Trend
- Availability Trend
- Breakdown Analysis

C. PBB Monitoring
- Breakdown Trend
- Serviceability Trend
- Availability Trend

### 4. Complaint Analytics

Using Airline Complaints sheet:

Display:

- Total Complaints
- Complaints by Equipment Type
- Complaints by Stand
- Complaints by Category
- Complaint Resolution Time
- Root Cause Analysis

Charts:

- Pareto Chart
- Monthly Complaint Trend
- Complaint Type Distribution
- Stand-wise Complaints

### 5. Breakdown Dashboard

Using Major Complaint-Breakdown and PBB Breakdown sheets:

Show:

- Total Breakdowns
- Breakdown Hours
- MTTR (Mean Time To Repair)
- Equipment-wise Breakdown Count
- Stand-wise Breakdown Count
- Open Issues
- Closed Issues

Charts:

- Breakdown Trend
- Breakdown Category Analysis
- Downtime Heat Map

### 6. Usage Analysis Dashboard

Using Usage Summary sheet:

Create:

- Daily Usage %
- Daily Non-Usage %
- Flight Count Trend
- Usage vs Non-Usage Trend
- Reason-wise Non-Usage Analysis

Charts:

- Pie Chart
- Bar Chart
- Trend Line Chart

### 7. Operator Performance Dashboard

Using Performance Report sheet:

Display:

- Total Operators
- Best Performing Operator
- Lowest Performing Operator
- Overall Usage %

Charts:

- Top 10 Operators by Usage %
- Operator Performance Ranking
- Usage vs Non-Usage Analysis
- Flights Handled per Operator

Provide operator scorecard.

### 8. Inventory Dashboard

Using Removed Item List sheet:

Show:

- Total Removed Parts
- Inventory by Category
- Frequent Component Failures
- Most Replaced Components
- Component Replacement Trend

### 9. Kaizen Dashboard

Display:

- Total Kaizens Implemented
- Kaizen Status
- Implementation Timeline
- Improvement Tracker

### 10. Data Tables

Every dashboard section should include:

- Search
- Filter
- Sort
- Export CSV
- Export Excel
- Pagination

### 11. Automated KPI Calculations

Implement automatic calculations.

Serviceability Formula:

((Total Running Hours × Number of Units) −
(PM Hours + Breakdown Hours))
/
(Total Running Hours × Number of Units)

Availability Formula:

((Total Running Hours × Number of Units) −
Breakdown Hours)
/
(Total Running Hours × Number of Units)

Allow formulas to be configurable. 【1-2d1382】

### 12. Dashboard UI Design

Create an executive-level dashboard with:

- Bootstrap 5
- Modern Airport Operations Theme
- Responsive Design
- Dark Mode
- Light Mode
- Interactive Charts
- KPI Cards
- Sidebar Navigation
- Drill-down Capability
- Professional Color Palette

Suggested Colors:

- Navy Blue
- Airport Grey
- White
- Green (Healthy KPI)
- Orange (Warning)
- Red (Critical)

### 13. Technical Stack

Frontend Only:

- HTML5
- CSS3
- JavaScript
- Bootstrap 5
- Chart.js
- DataTables.js
- SheetJS (xlsx)

### 14. Deliverables

Generate:

1. Complete single-page HTML application.
2. Embedded CSS.
3. Embedded JavaScript.
4. Excel Upload functionality.
5. Automatic worksheet detection.
6. Dynamic KPI calculations.
7. Dynamic chart generation.
8. Executive dashboard layout.
9. Fully responsive design.
10. Professional production-ready code.

Output Requirement

Generate complete working code, not pseudocode.

The dashboard should automatically parse uploaded Excel files having structures similar to the attached Airport KPI workbook and immediately populate all KPI cards, charts, tables, and management reports without requiring backend development.
