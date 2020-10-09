# FeatureEngineering

## Variable Characteristics
- Missing Data 
- Categorical Variables
- Linear Model Assumptions - Do the variables fulfill those assumptions? 
- Distributions - Normal, skewed, and others
- Outliers
- Feature Magnitude - Scale of the different features
## Dates and Time Variables

#### Dates
- Day
  - Name - Mon, Tue, Wed,...
  - Number - 1-7
  - IsBusinessDay, IsHoliday, IsWeekend
- Month
  - Name -Jan, Feb, March,...
  - Number - 1-12
  - Quarter
  - Semester
- Year

#### Times
- Hour
  Did TS take place in morning, afternoon, night
- Minutes
- Seconds

#### Date/Time difference in:
- Days
- Months
- Years
- Hrs
- Minutes
- Seconds

#### Consider time zones
Payment data 1 ('29-08-1987 15:20.20+02') ---> Payment data 1 ('29-08-1987 13:20.20+00')
Payment data 2 ('29-10-1993 15:20.20+05') ---> Payment data 2 ('29-10-1993 10:20.20+00')
## Mixed Variables
