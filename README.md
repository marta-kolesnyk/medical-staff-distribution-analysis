# Analysis of the Medical Staff Distribution Across the U.S. for Upcoming Flu Season

# Overview: 
During the flu season in the United States, there's a higher number of people getting sick, especially those in vulnerable groups, who might need hospitalization due to serious complications. Hospitals and clinics require extra staff to handle the increased number of patients, which is provided by medical staffing agency.

# Objective: 
Determine when to send staff, and how many to each state.

# Scope: 
The agency covers all hospitals in each of the 50 states of the United States, and the project planned for the upcoming influenza season.

# Key Questions:
- What data is needed to inform the timing and spatial distribution of medical personnel throughout the United States?
- Determine whether influenza occurs seasonally or throughout the entire year. Does it start and end in the same month in every state?
- Prioritize states with large vulnerable populations. Consider categorizing each state as low-, or high-need based on its vulnerable population count.
  
# Data Used:
- Population Data by Geography (source: https://www.census.gov/data.html)

Includes yearly population counts for the U.S. counties from 2009 to 2017.
- Influenza Deaths Dataset (source: https://wonder.cdc.gov/ucd-icd10.html)
Includes monthly flu death counts for each state from 2009 to 2017. Death counts of 9 or fewer people are not allowed to be published, therefore were suppressed (81.7% of the records).
# Data Limitations:
- As 80% of death count data was suppressed and imputed with random values (0-9), the real death counts could have been lower/higher, especially for the age group <5 years, as all their data was suppressed.
- Death counts for all age groups come from death certificates, that list only one cause of death. If a person had multiple health issues, including flu (or caused by flu), only one issue will be specified. As a result, actual flu-related death counts could be higher.

# Project Limitations:
- Having data on the vaccination status of vulnerable population groups would help to analyze the impact of vaccination on flu mortality rates across states. Also, information regarding the number of times people got vaccinated during the year would be useful, as I could compare mortality rates between two groups of people (with one and two doses of vaccine), especially in the states with irregular flu season.
- A monthly doctor-to-patient ratio would be helpful in determining states that are in need of additional personnel and adjusting the number of personnel for the next month.


# Project Deliverables:
- Project management plan
- Interim report
- Final presentation in a form of Tableau storyboard
- Video presentation: https://go.screenpal.com/watch/c0iZbcVkIdI

