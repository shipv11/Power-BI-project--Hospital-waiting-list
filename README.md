# PowerBIproject-HospitalWaitingList
Analysis of a publicly available dataset from Ireland about the waiting list of patients requiring treatment from a few hospitals between 2018 and 2021.
## Objectives:
•	Track current status of patient waiting list.
•	Analyse historical monthly trend of waiting list in Inpatient and Outpatient categories.
•	Detailed speciality level and age profile analysis.

**Metrics**- Average and Median waiting list, current total waiting list.
**Views made**- Summary page and detailed page for granular analysis.

## Data collection
- Combined and loaded Inpatient data from the years 2018 to 2021 in a single table. Done the same for outpatient data.
Renamed column “speciality” in inpatient data.
Added a new column case type as outpatient in outpatient table
Appended the queries to create a new table that contains all the data.
In power query editor, standardised the time bands column by removing spaces and correcting spellings using trim and replace.
Designed blueprint of summary and detail pages

## In the summary page:
Created latest month wait list measure and previous year latest month wait list (using edate) and displayed them with cards
Created new table ‘calc method’ with two values- average and median and then created a slicer with this table.
Created two new measures- average wait list and median wait list
Created Avg/med wait list measure which uses switch to switch between these two measures.
Created a donut chart showing avg/median wait list by case type.
Displayed clustered column chart showing avg/med wait list by time bands and age profile. Filtered blank values.
Created a multi-row card showing Top 5 speciality with the highest avg/med wait list
Created two line charts showing the trend of the total waiting list over the four years with respect to inpatient vs outpatient numbers.
Created 3 slicers for date, case type and speciality.

## In the detailed view page:
Created a matrix showing inpatient and outpatient information in detail with respect to specialty, time bands and age profile.
Added background and formatted charts for better visibility
Added page navigation

## Conclusion: 
The waiting list increased from last year.
The vast majority of waiting people are outpatient cases.
A big majority of people have to wait either less than three month or more than 18 months.
Majority of waiting patients are between the ages of 16-64.
While the trend in inpatient cases has remained mostly stable, the trend of outpatient cases has been steadily increasing.
