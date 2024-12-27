# Titanic-Survival-Analysis
Analyze the Titanic dataset to uncover patterns influencing passenger survival. 

## Introduction
### Purpose
This project analyzes the Titanic dataset to identify factors that influenced passenger survival during the disaster.

### About the Dataset
The dataset contains demographics and passenger information from 891 of the 2,224 passengers and crew on board the Titanic. It includes features such as:

+ Passenger Class (Pclass)
+ Sex
+ Age
+ Siblings/Spouses Aboard (SibSp)
+ Parents/Children Aboard (Parch)
+ Ticket Number
+ Fare
+ Cabin
+ Embarked
+ Survival Status (Survived)
The dataset is sourced from [Kaggle](https://www.kaggle.com/datasets/yasserh/titanic-dataset)

## Analysis Questions
The analysis aims to answer the following questions:

1. Which factors significantly influenced survival rates?
+ Gender
+ Passenger Class
+ Age
+ Family Size
2. How did embarkation point affect survival?
3. What role did fare play in survival likelihood?

## Setup Instructions
1. Clone the repository:
   ```
   git clone https://github.com/26vyshnavi/Titanic-Survival-Analysis
   cd Titanic-Survival-Analysis
   ```
2. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```
3. Run the Jupyter Notebook or Python script:
   ```
   jupyter notebook Titanic-Survival-Analysis.ipynb
   ```

## Methodology
### Data Wrangling
1. Missing Values:
- Identified and handled missing values in Age, Cabin, and Embarked columns.
- Used median imputation for Age and mode imputation for Embarked.
- Dropped the Cabin column due to a high percentage of missing values.

2. Feature Engineering:
- Created a new feature FamilySize by summing SibSp and Parch.
- Generated IsAlone feature to indicate if a passenger was alone.
  
### Exploratory Data Analysis (EDA)
1. Survival Rates by Gender and Class:
- Visualized survival rates across different genders and passenger classes.

2. Age Distribution:
- Plotted age distributions to observe survival trends among different age groups.

3. Embarkation Points:
- Analyzed survival rates based on embarkation points (C, Q, S).

4. Fare Analysis:
- Examined the relationship between fare amounts and survival.

### Statistical Analysis
1. Correlation Matrix:
- Computed correlations between numerical features and survival status.
  
2. Hypothesis Testing:
- Conducted statistical tests to determine the significance of observed patterns.

## Key Findings
1. Gender:
- Females had a significantly higher survival rate than males.

2. Passenger Class:
- First-class passengers were more likely to survive compared to second and third classes.

3. Age:
- Younger passengers had higher survival rates, particularly children.

4. Family Size:
- Passengers with small family sizes had better survival chances than those alone or with large families.

5. Embarkation Point:
- Passengers who embarked from Cherbourg (C) had higher survival rates.

6. Fare:
- Higher fares correlated with increased survival likelihood, possibly due to association with higher classes.

## Conclusion
The analysis indicates that survival on the Titanic was influenced by multiple factors, including gender, class, age, family size, embarkation point, and fare. These insights align with historical accounts of the disaster, where women, children, and upper-class passengers were given priority during evacuation.
