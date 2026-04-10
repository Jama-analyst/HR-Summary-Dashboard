# HR-Summary-Dashboard
This HR Summary Dashboard provides a high-level overview of the organization’s workforce, focusing on demographics, departmental distribution, and financial metrics across all global operations.

## Key Performance Indicators (KPIs)
The organization maintains a workforce of 1,470 employees (1.47K) with the following averages:
- Average Monthly Income: 6.5K
- Average Monthly Rate: 14.3K
- Average Job Experience: 13.92 years

## Workforce Composition
- [X] Gender Diversity
The workforce shows a significant gender lean, with 60% identifying as Female and 40% as Male. This ratio remains relatively consistent across various departments, though the total volume of employees varies.

- [X] Marital Status
The employee population is predominantly composed of married individuals:
- Married: 45.6%
- Single: 32.1%
- Divorced: 22.3%

## Departmental Insights
The dashboard utilizes numerical identifiers for departments (1 through 6).
- Employee Count: Department 6 is the largest by a wide margin, employing over 400 individuals. Department 1 is the smallest, with fewer than 100 employees.
- Income Distribution: While Department 6 has the highest headcount, Department 4 appears to command the highest average monthly income, peaking at approximately 7,604.88 for male employees.
- Gender Pay Parity: In most departments, the average monthly income between male and female employees is closely aligned, suggesting equitable pay structures across the numerical divisions.

## Engagement Factors
The "Factors Affecting Job Experience" radar chart indicates multiple data points influencing the employee lifecycle. While specific labels are minimized, the distribution suggests that job experience is influenced by a balanced mix of internal factors rather than a single outlier.

## Obversation
The organization possesses a highly experienced workforce (averaging nearly 14 years). This suggests high retention rates, though it may also indicate a need for succession planning as senior staff approach retirement.

## HR Summary Dashboard
![image](https://github.com/Jama-analyst/HR-Summary-Dashboard/blob/main/HR%20Summary%20Dashboard.png)

[Team Roug Sketches](https://github.com/Jama-analyst/Business-Insight-360/blob/main/Team%20Rough%20Sketches.png)

## Tech Stacks
- [X] IBM Cognos Analytics Tool
- [X] HR_DATASET.csv
- [X] Excel


## Project Charter File
- PowerBI techniques Learnt
- What are all the questions should be asked before staring the project
- Creating calculated columns
- Creating measure using DAX language
- Data modeling
- Using Bookmarks to switch between two visuals
- Page navigation with buttons
- Using divide function to prevent zero division errors
- Creating date table using m language
- Dynamic titles based on the applied filters
- Using KPI indicators
- Conditional formatting the values in visuals using icons or background color
- Data validation techniques
- PowerBI Services
- Publishing Reports to PowerBI Services
- Setting up personal gateway to set up the auto refresh of data
- PowerBI App creation
- Collaboration, workspace, access permissions in PowerBI Services
- And more 😅
  
## GitHub
Uploading Large size files using GitHub LFS
Tracking the particular type of file extensions for LFS

## Key KPIs
- Gross Price
- Pre-invoice deductions
- Post-Invoice deductions
- Net Invoice Sale
- Gross Margin
- Net Sales
- Net Profit
- COGC (Cost of Goods Sold)
- YTD (Year to Date)
- YTG (Year to Go)
- Direct
- Retailer
- Distributors
- Consumer

Project kick off session, where you should get clear of for what and why this project and all other questions you have with regards to the project

## Questions to ask before starting with dashboard
- [X] Being Proactive
       - As a Data Analyst, one needs to ask questions, as one needs clarification from the begining
- [X] NB! One should worry about the authority (in terms of the Stakeholders) of the person that you are talking to. If one is being very clear and upfront it's gonig to help everybody.
- [x]	Expectation Management
       - Setting Realsitic Expectation e.g. Feature Creep (Tony wanted to make it very clear, that he'll not allow making to many changes while the project is on
- What is the objective of building this PowerBI Dashboard?
- In what terms the success of this project will be measured?
- What will be time dead-line of the project?
- Do the stakeholders expecting pre-view before the actual release?
- What are all the hopes stakeholders have out of this project?
- What are all fears the stakeholderS have in terms of building this dashboard?
- Who are all will be using this dashboard and for what purpose?
- What are all expectation the stakeholders have, by the completion of this project?
- What can go wrong while building this project?
- What are all the resources/ data needed to build this dashboard?
- Is there any inputs from stakeholders in terms of design and views of the dashboard?
  
After the project kick off meetings, the data engineering team has given the data as per the request of data analytics team, let’s explore them.

## Dataset Understanding.
Understanding what data is available will be more helpful while doing analysis, before jumping on to the analysis one needds to get a good understanding of what data are available.

- [X] Dimension Table : It will have the static data like details of customer and products

- [X] Fact Table : It will have the data about the transactions

gdb041:
- [X] dim_customer
- distinct markets (ex India, USA, Spain)
- 75 distinct customers thorough out the market
- [ ] 2 types of platforms
- Brick & Motors - Physical/offline store
- E-commerce - Online Store (Amazon, flipkart)
- [ ] Three channels
- Retailer
- Direct
- Distributors
- [X] dim_market
- 27 distinct markets (ex India, USA, spain)
- 7 sub-zones
- [ ] 4 regions
- APAC
- EU
- nan
- LATAM
- [X] dim_product
- [ ] Divisions
- [ ] P & A
- Peripherals
- Accessories
- [ ] PC
- Notebook
- Desktop
- [ ] N & S
- Networking
- Storage
 [ ]  There are 14 different categories, Like Internal HDD, keyboard
 [ ] There are different variants available for the same product
- [X] fact_forecast_monthly
- [ ] This table is used to forecast the customer’s need in advance, which can help in
 - Higher customer satisfaction
 - Reduced cost in warehouses for storage purpose
- The table is denormalized by data engineering team, as it is a data warehouse which is aimed to be used for analytical work.
- All the date of the month will be replaced by the start date of the month
- It will have all the column names and in the end it will have the forecast quantity need of the customer
- [X] fact_sales_monthly
- This table is more or less is same as fact_forecase_monthly table, but the last column has the value of sold quantity instead of forecast value.

gdb056
- [X] freight_cost
- This table has details of travel cost and other cost for each market with fiscal year
- [X] gross_price
- Has the details of gross prices with product code
- [X] manufacturing_cost
- Has the details of manufacturing cost with product code with year
- [X] Pre_invoice_dedutions
- Has the details of pre invoice deductions percentage for each cutomer with year
- [X] Post_invoice_deductions
- Post invoice deductions and other deductions details

## Importing data into PowerBi
As the database is MySQL in this project, we need to import the datasets from MySQL database to PowerBI by providing the Database access credential

## Data Model
- Data Modeling plays a vital role and is considered as the basement of report. All the visuals will be build upon the data model.
- Poor Data Modeling affects the over all performance of the report.
- Following Good practices of Data Modeling is must. 
- In this project, we have followed Snowfall Data Modeling method.
  
[Data Model](https://github.com/Jama-analyst/Business-Insight-360/blob/main/Data%20Model.png)


## Dashboard designing
Based on the Mock-ups received as requirement, the team will start designing the visuals and create measure as and when required
   - Benchmark Data
   - A Mock-up/Rough Dashboard (how the dashboard should look like for Finance View, Executive View, etc) to use it for reference.
     
[Rough Dashboard Sketches](https://github.com/Jama-analyst/Business-Insight-360/blob/main/rough-dashboard-sketch.pdf)
          
[Benchmark Data](https://github.com/Jama-analyst/Business-Insight-360/blob/main/benchmark-numbers.docx)

## Country Australia
In Home View, all the views button will be available. User will land on specific view page by clicking the button
[Home View](https://github.com/Jama-analyst/Business-Insight-360/blob/main/Home%20Page.png)

## Info Page
[Info Page](https://github.com/Jama-analyst/Business-Insight-360/blob/main/Info%20Page.png)

## Finance View
[Finance View Dashboard](https://github.com/Jama-analyst/Business-Insight-360/blob/main/Finance%20View%20Dashboard.png)

## Sales View
[Sales View Dashboard](https://github.com/Jama-analyst/Business-Insight-360/blob/main/Sales%20View%20Dashboard.png)

## Marketing View
[Marketing View Dashboard](https://github.com/Jama-analyst/Business-Insight-360/blob/main/Marketing%20View%20Dashboard.png)

## Supply Chain View
[Supply Chain View Dashboard](https://github.com/Jama-analyst/Business-Insight-360/blob/main/Supply%20Chains%20View%20Dashboard.png)

## Executive View
[[Executive View Dashboard](https://github.com/Jama-analyst/Business-Insight-360/blob/main/Executive%20View%20Dashboard.png)

## Support Page
[Support Page](https://github.com/Jama-analyst/Business-Insight-360/blob/main/Support%20Page.png)

