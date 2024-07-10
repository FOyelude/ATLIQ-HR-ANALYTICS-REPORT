# ATLIQ-HR-ANALYTICS-REPORT
ATLIQ HR ANALYTICS REPORT with PowerBI

## Project Description
The objective was to analyze employees' working preferences, understand the percentage of sick leaves taken, and gain insights into various leave trends to help the HR department optimize workforce management and enhance productivity.

## Process to Discover and Present Meaningful Insights

### Data Loading
- Loaded the employee data into Power BI to start the analysis.

### Data Transformation
- **Filtering Data**: Filtered the data to include only April, ensuring the analysis was specific to this period.
- **Table Duplication**: Duplicated the table to have a working copy for all necessary transformations while preserving the original data.
- **Header Promotion**: Promoted the first row to headers for better data organization.
- **Row Removal**: Removed the top row to clean the dataset.
- **Column Renaming**: Renamed the columns to more meaningful names for clarity and consistency.
- **Data Unpivoting**: Selected the employee code and name columns and unpivoted other columns to restructure the data for easier analysis.
- **Invalid Rows Removal**: Changed the data type of the date column to DATE to identify and remove invalid rows by filtering out errors, automating the process for future data updates.
- **Parameter Creation**: Created a parameter to dynamically filter the sheet names.
- **Function Creation**: Created a function called GetData from the template table. Changed the filter of the template column to use the parameter instead of text, ensuring flexibility and automation.
- **Function Invocation**: Applied the GetData function using 'Invoke Custom Function' on the original data to transform it accordingly.
- **Column Cleanup**: Removed unnecessary columns to streamline the dataset and focus on relevant information.
- **Final Data Load**: Loaded only the transformed and clean data into Power BI for analysis and visualization.

### Building the Dashboard
- **Measure Creation**: Developed various measures such as Actual Working Days, Total Present Days, Work from Home, Present Onsite, Sick Leave Counts and Percentages, among others. These measures provided critical metrics for analysis.
- **New Columns Addition**: Added new columns to account for half days and full days (e.g., Half Work from Home and Work from Home) using 0.5 for half days and 1 for full days, ensuring accurate representation of work hours.
- **Advanced Filtering**: Used advanced filtering techniques to remove days not present in the data and days off, refining the analysis to focus only on relevant working days.

### Key Insights
- **Special Leave Analysis**: Menstrual leaves had the highest percentages among all special leaves, indicating a significant need for accommodating this type of leave.
- **Sick Leave Trends**: Sick leaves were taken most frequently in June, suggesting possible seasonal trends or health-related issues during this month.
- **Work from Home Patterns**: Employees worked from home the most on Fridays, highlighting a preference for remote work at the end of the week.
- **Onsite Presence**: Employees were more present onsite on Tuesdays and least on Fridays, which could inform scheduling and resource allocation.
- **Workplace Ratio**: There was a 90% onsite presence compared to 10% working from home, providing a clear picture of the overall work environment.
- **Monthly Trends**: There were more work-from-home instances in May than any other month, which could indicate specific factors influencing remote work during this period.

By leveraging Power BI for data transformation and visualization, I provided Atliq Technologies' HR department with actionable insights to optimize workforce management, improve employee satisfaction, and enhance overall productivity.


