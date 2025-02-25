# HR Employee Joining Analysis

## Project Overview
This project analyzes HR data to understand why employees join a company. It explores factors such as notice periods, salary hikes, joining bonuses, and job roles to provide insights into employee decisions.

## Dataset
The dataset includes various attributes related to job offers, candidate expectations, and final decisions. Key columns include:
- **DOJ Extended**: Whether the Date of Joining was extended.
- **Duration to accept offer**: Time taken by the candidate to accept the offer.
- **Notice period**: Notice period required by the candidate.
- **Offered band**: Job level/grade offered to the candidate.
- **Percent hike expected in CTC** vs. **Percent hike offered in CTC**: Difference between expected and offered salary hikes.
- **Gender**: Candidate's gender.
- **Candidate relocate actual**: Willingness to relocate for the job.
- **Candidate Source**: Recruitment channel.
- **Rex in Yrs**: Relevant experience in years.
- **LOB**: Line of business/department the candidate will join.
- **Status**: Whether the candidate joined or not.

## Exploratory Data Analysis (EDA)
### 1. General Data Insights
- Checked for missing values and data types.
- Descriptive statistics for numerical columns.

### 2. Visualizations
- **DOJ Extended Analysis**: Count plot to see how many candidates had their joining date extended.
- **Offer Acceptance Time**: Histogram to analyze how long candidates take to accept offers.
- **Notice Period vs. Offer Acceptance**: Bar plots and scatter plots to understand urgency in hiring.
- **Offered Band Distribution**: Pie chart to visualize the distribution of job levels.
- **Salary Hike Expectations vs. Reality**: Distribution plots comparing expected and offered hikes.
- **Joining Bonus Trends**: Analysis of job positions where joining bonuses are offered.
- **Gender-based Hiring Trends**: Pie charts and bar plots.
- **Relocation Trends**: Bar plots analyzing employee relocation decisions.
- **Recruitment Channels**: Bar plot showing the most common hiring sources.
- **Experience vs. Salary Hike**: Analysis of how years of experience affect salary hike negotiations.
- **Department-wise Hiring Trends**: Bar chart for department-wise candidate distribution.

### 3. Key Insights
- **Salary Hike Expectations**: On average, the percent hike offered is lower than what candidates expect.
- **Age Distribution**: The average candidate age is ~29.9 years, with most candidates aged 30+.
- **Offer Acceptance Time**: Candidates take an average of 21 days to accept an offer.
- **Experience Levels**: Most candidates have low relevant experience (~4.24 years on average).
- **Notice Period Trends**: 30-day notice periods are the most common, and longer notice periods reduce the likelihood of candidates joining.
- **Recruitment Sources**: Majority of candidates are sourced directly by the company.
- **Location Trends**: Chennai has the highest number of candidates and joinees.
- **Gender Distribution**: Majority of candidates are male.
- **Job Levels**: E1 offer band is the most common among employers.

## Machine Learning Models
### 1. Data Preprocessing
- Handled class imbalance using **SMOTEENN**.
- Normalized data using **MinMaxScaler**.

### 2. Logistic Regression Model
- Achieved an accuracy of **83.38%**.
- ROC AUC score: **0.837**.
- Confusion matrix plotted for model evaluation.

### 3. Random Forest Classifier
- Achieved an accuracy of **83.04%**.
- ROC AUC score: **0.821**.
- Feature importance analysis performed.

### 4. Other Models Tested
- **AdaBoost Classifier**
- **Gradient Boosting Classifier**
- **Extra Trees Classifier**
- **Naive Bayes (BernoulliNB)**
- **Decision Tree Classifier**
- **K-Nearest Neighbors (KNN)**

## Conclusion
- Candidates with shorter notice periods are more likely to join.
- The offered salary hike is usually lower than expected, impacting candidate decisions.
- Direct sourcing is the most effective recruitment strategy.
- Chennai has the highest number of hires.
- Machine learning models provide good accuracy in predicting whether a candidate will join.
