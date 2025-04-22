### MADSCapstone25 - Team 22 Math Educators
# Capstone Project - Improving Visual Feedback for Students through Machine Learning Analysis
### Peter Bloomsburgh (peterblo@umich.edu) and Emily McClear (emcclear@umich.edu)

This resposity contains the code and data used for our capstone project analyzing student data from Peter's website, algebra123.org to improve visual feedback with student and mentor progress reports. 

## Repository Structure

### Notebooks
Our ML analysis is broken down across six Jupyter notebooks, created in Google Colab. The notebooks are executed in the following order: 
1. **ML Data Processing** - Prepares raw data for analysis, including cleaning, feature engineering, merging, train/test splitting, and downloading.
2. **ML Mastery Statistics** - Analyzes mastery metrics mastery and probs_before_mastery.
3. **ML Panel Regression** - Implementes PooledOLS, Fixed Effects, and Random Effects models on prepared panel data to predict probs_before_mastery
4. **ML Performance Statistics** - Measures and visualizes student accuracy across all problems and over quizzes only.
5. **ML Forecasting** - Predicts future daily average quiz performance using an ARIMA model.
6. **ML Session Clustering** - Defines user sessions and applies KMeans Clustering techniques to identify session patterns.

### Data

#### Raw Data Files
These are the original data files pulled from Peter's database for algebra123.org records: 
- 'k8_mastery-3.csv' contains parameters detailing when students achieve mastery
- 'k8_probs-2.csv' contains parameters detailing each problem attempted by any student from August 2024 to April 2025.
- 'k8_quizzes-2.csv' contains parameters detailing each quiz submitted by any student from August 2024 to April 2025.

#### Cleaned Data Files
Cleaned and structured versions of the raw data are stored in four sets of files: 
- 'mastery_csv' contains cleaned and standardized parameters describing when students achieve mastery
- 'merged_csv', 'merged_test.csv', and 'merged_complete.csv' contain the train, test, and complete (respectively) cleaned and standardized parameters describing each valid problem completed, both as practice and within a quiz
- 'prob_csv', 'prob_test.csv', and 'prob_complete.csv' contain the train, test, and complete (respectively) cleaned and standardized parameters describing each valid problem completed as practice
- 'quiz_csv', 'quiz_test.csv', and 'quiz_complete.csv' contain the train, test, and complete (respectively) cleaned and standardized parameters describing each valid quiz completed

## Project Objective
The primary goal of this project is to evaluate and model student learning behaviors using data derived from real-student interactions with Peter's web-based mathematics resource, and to apply these insights to provide better feedback to students by improving visualizations in the student and mentor progress reports. Topics of analysis include: 
- Educational/web data preprocessing
- Mastery learning metrics
- Panel regression modeling
- ARIMA predictive modeling
- Clustering user sessions

## Code and Data Access Statements

### Code Access
Any code currently deployed or in production for **algebra123.org** is proprietary material owned by **Peter Bloomsburgh**. While it is not publicly available in this repository, it may be reviewed upon request. Please email **peterblo@umich.edu** for more information. 

### Data Access
All data used in this project was independently scraped from **algebra123.org** and stored by **Peter Bloomsburgh**. The exact datasets used for project analysis are included in the raw data files listed above. 

## Contact
For questions, contact Emily McClear (emcclear@umich.edu) or Peter Bloomsburgh (peterblo@umich.edu)
