# FeatureEngineering

## Variable Characteristics
- Missing Data 
- Categorical Variables
- Linear Model Assumptions - Do the variables fulfill those assumptions? 
- Distributions - Normal, skewed, and others
- Outliers
- Feature Magnitude - Scale of the different features

#### Cardinality
  - Strings are incompatible with Scikit-Learn
  - Variables with high cardinality OR Uneven Distibution  between train and test sets results in overfitting in tree based algorithms and operational problems
    - Reducing cardinality may help improve model performance
    - Error in operation/production occur  becuase the model is learning from the labels seen in the train set and a new unseen label comes then thhe model will be un able to perform calculation

## Variable Transformation (Normality)
 Mathematical transformations
 - Logarithmic - Log(X) --> x>0
 - Reciprocal - 1/X -->x!=0
 - Power/Exponential X exp(lambda)/sqrt(X)/cube(X) --> Not defined foe all x
 - Exponential special cases - Box Cox(x>0)/Yeo Johnson

## Discretisation 
Discretisation(Binning) is the process of transforming continious variables into discrete variables by creating a set od intervals that span the range of the variables values
Discretisation helps handle outliers and may improve value spread in skewed variables.

####  Unsupervised discretisation methods

- Equal width discretisation
- Equal frequency discretisation
- K-means discretisation

#### Supervised discretisation methods

- Discretisation using decision trees

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
