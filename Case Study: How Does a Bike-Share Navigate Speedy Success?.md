# Case Study: How Does a Bike-Share Navigate Speedy Success?

## Scenario
You are a data analyst working on the marketing analyst team at Cyclistic, a bike-share company in Chicago. The director of marketing believes the company's future success depends on maximizing the number of annual memberships. Therefore, your team wants to understand how casual riders and annual members use Cyclistic bikes differently. From these insights, your team will design a new marketing strategy to convert casual riders into annual members. But first, Cyclistic executives must approve your recommendations, so they must be backed up with compelling data insights and professional data visualizations.

### Business Task
Analyze how casual riders and annual members use Cyclistic bikes differently and design a new marketing strategy to convert casual riders into annual members.

### Data Sources
Cyclistic’s historical trip public data for the last 5 years. For my research, I used data from 2023 (total number of records: 2.5M).

## Purpose and Context
I’m analyzing a dataset from a bike-sharing company to understand usage trends. The goal is to identify patterns, anomalies, and prepare the data for further analysis.

## Data Cleaning Techniques Used

- **Data Validation:**
    - Checked for missing values and ensured data consistency.
    - Validated that timestamps were in the correct format.
- **Data Screening:**
    - Examined trip duration outliers (e.g., rides lasting over 24 hours).
    - Investigated unusually high or low bike usage counts.
- **Data Diagnosing:**
    - Explored inconsistencies in station names (e.g., typos, variations).
    - Detected duplicate records based on ride IDs.
- **De-duplication:**
    - Removed duplicate entries to maintain data integrity.
- **Handling Invalid Data:**
    - Flagged records with negative trip durations as erroneous.
- **Addressing Outliers:**
    - Capped trip durations at 24 hours.
    - Removed rides with extreme start/end coordinates.

## Workflow and Steps
1. Loaded raw data from CSV files into MySQL using MySQL Workbench.
2. Cleaned timestamp formats and converted them to datetime objects.
3. Validated ride IDs and station names.
4. Created new features (e.g., day of the week, season).
5. Visualized usage patterns using Tableau.

## Challenges and Solutions
- **Inconsistent Station Names:**
  - Solution: Created a mapping dictionary to standardize station names.
- **Negative Trip Durations:**
  - Solution: Investigated and corrected data entry errors.

## Data Exclusions
- Excluded records with incomplete information (e.g., missing start/end stations).
- Removed outliers beyond reasonable trip durations.

## Summary
In this project, I explored usage trends for a bike-sharing company. I used Tableau for visualization and MySQL to transform the data. The result was a comprehensive dashboard highlighting key insights.

## Methods Used
1. **Data Exploration and Transformation:**
   - Analyzed a substantial dataset comprising 2.5 million records.
   - Leveraged MySQL to clean and transform the data.
2. **Data Visualization:**
   - Utilized Tableau to create an interactive dashboard.
   - Highlighted key insights for stakeholders.

## Key Findings
1. **User Types:**
   - Non-members (casual riders) constituted 25% of the total ridership.
   - Non-members tended to take longer trips compared to members.
2. **Activity Patterns:**
   - Non-members were more active on Fridays and weekends, suggesting potential tourists.
   - They often picked up bikes in touristic areas.
3. **Bike Preferences:**
   - Non-members preferred standard bikes over electric ones.

## Recommendations
### Membership Promotion:
- Encourage non-members to become members by offering incentives such as discounted rates for the first month or free trial periods.
- Highlight the benefits of membership, such as shorter wait times, priority access to bikes, and exclusive offers.
### Tourist Engagement:
- Since non-members are often active on weekends and in tourist areas, consider targeted marketing campaigns for tourists.
