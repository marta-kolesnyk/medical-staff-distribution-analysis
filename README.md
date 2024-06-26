# Analysis of the Medical Staff Distribution across the U.S. for Upcoming Flu Season

## Overview: 
During the flu season in the United States, there's a higher number of people who might develop serious complications and will require hospitalization. Hospitals and clinics need extra staff to handle the increased number of patients. Medical staffing agency aims to send the reasonable number of the additional personnel.

## Objective: 
Determine when to send staff, and how many to each state.

## Scope: 
The agency covers all hospitals in each of the 50 states. The project is planned for the upcoming flu season.

## Key Questions:
- What data is needed to inform the timing and spatial distribution of medical personnel throughout the United States?
- Determine whether influenza occurs seasonally or throughout the entire year. Does it start and end in the same month in every state?
- Prioritize states with large vulnerable populations. Consider categorizing each state as low-, or high-need based on its vulnerable population count.
  
## Data Used:
- **Population Data by Geography** (source: https://www.census.gov/data.html)
Includes yearly population counts for the U.S. counties from 2009 to 2017.

- **Influenza Deaths Dataset** (source: https://wonder.cdc.gov/ucd-icd10.html)
Includes monthly flu death counts for each state from 2009 to 2017.

## Data Limitations:
- Death counts of 9 or fewer people are not allowed to be published, therefore were suppressed (81.7% of the records).
- As suppressed values were imputed with random values (1-9), the real death counts could have been lower/higher, especially for the age group <5 years, as data all for this category was suppressed.
- Death counts for all age groups come from death certificates, that list only one cause of death. If a person had multiple health issues, including flu (or caused by flu), only one issue will be specified. As a result, actual flu-related death counts could be higher.

## Data Cleaning Process:
- Both datasets were checked in Excel for data accuracy and consistency using **descriptive statistics** and **Pivot Tables**. Inconsistent state namings were replaced.
- Removed duplicate records from Population dataset (used **data grain level** County-State-Year).
- Replaced suppressed values in Flu Deaths Dataset with the random numbers from 1 to 9, since this data was crucial for the future analysis.
- Aggregated data by states and years using Pivot Table, transformed data.
- Combined two datasets using **VLOOKUP() function**.
- Normalized flu data according to state population.

## Analysis Phases:
  - Created a research hypothesis, determined the measures of spread for the key variables (standard deviation, mean, outliers).
  - Conducted statistical hypothesis testing using t-test in Excel.
  - Created temporal and spatial visualizations in Tableau.
  - Presented key findings and recommendations as a storyboard.
 
## Main Findings and Recommendations:
- The research hypothesis was confirmed - Flu death rates for vulnerable populations (under 5 and over 65 years) is higher than the death rates for the rest of the population (5-64 years). 
- The medical agency should prioritize states where flu mortlaity rates for vulnerable groups are higher than the country average (more than 0.12%). 13 states were listed as high-need.
- Mentioned states have irregular flu seasons, with a couple of peak months that change from year to year. Medical personnel should be sent to these places in equal proportions all year round and KPIs (death rate and doctor-to-patient ratio if possible) should be monitored to redistribute the staff when needed.

## Project Limitations:
- Having data on the vaccination status of vulnerable population groups would help to analyze the impact of vaccination on flu mortality rates across states. Also, information regarding the number of times people got vaccinated during the year would be useful, as I could compare mortality rates between two groups of people (with one and two doses of vaccine), especially in the states with irregular flu season.
- A monthly doctor-to-patient ratio would be helpful in determining states that are in need of additional personnel and adjusting the number of personnel for the next month.

## Project Deliverables:
- Project management plan
- Interim report
- Final presentation in a form of Tableau storyboard
- Video presentation

