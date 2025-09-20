**CAPSTONE PROJECT - EMPLOYEE PERFROMANCE PREDICITON**

**Initial Data Analysis and Exploratory Report**
This report provides an initial exploratory data analysis (EDA) of the EmployeesPerformanceDataset.csv data. The analysis focuses on understanding the data structure, identifying key metrics, and visualizing performance trends.

1. **Data Overview and Cleaning**
The dataset, which contains performance evaluation records, was loaded successfully.

The initial inspection revealed several key characteristics:
**Shape**: The dataset consists of 422 rows and 15 columns.
**Data Types**: Most columns are of object type (text). 
The score column, which is critical for analysis, is of type float64.
Completed date column was converted to datetime objects for easier manipulation and potential time-series analysis.
**Missing Values**: The Notes column was completely empty (100% missing values), so it was dropped. Other columns like 

**Score**, **Evaluee**, and **Evaluator** had no missing values after the initial cleaning process.

**Column	Missing Value Percentage**
**Notes	100.0%
Completed date	0.0%
Scale selected	0.0%
Performance indicator	0.0%
Result area	0.0%
Type of evaluation	0.0%
Evaluation title	0.0%
Project/Duration	0.0%
Evaluation level	0.0%
Team	0.0%
Evaluator	0.0%
Job title	0.0%
Person code	0.0%
Evaluee	0.0%
Score	0.0%**

2. **Key Findings from Descriptive Statistics**
An analysis of the numerical Score column provides a summary of performance ratings across the dataset:

**Average Score**: The mean score is approximately 6.67.
**Median Score**: The median score is 7.0, which is slightly higher than the mean, suggesting the data is either evenly distributed or slightly skewed towards higher scores.
**Standard Deviation**: With a standard deviation of 2.12, the scores show a moderate spread around the average.
**Score Range**: Scores range from a minimum of 1.0 to a maximum of 10.0. The most common score is 7, with a count of 127 records.

**Metric	Score Value**
count	422.000000
mean	6.671564
std	2.122176
min	1.000000
25%	5.000000
50%	7.000000
75%	8.000000
max	10.000000

3. **Distribution of Categorical Features**
The categorical features provide insights into the structure of the evaluations and the roles of the individuals involved.

**Job Title**: The dataset includes evaluations for a diverse range of roles, with PHP Developer being the most frequently evaluated position.
**Evaluation Level**: The most common evaluation type is Downward, which typically involves a manager evaluating an employee. 
Peer and Self evaluations also make up a significant portion of the dataset.
**Performance Categories (Scale selected)**: The most common performance rating is Adequate, indicating that most employees are meeting expectations. Ratings like 

Needs Improvement and Sometimes Meets Expectations also appear frequently.

**Evaluation Level	Count**
Downward	280
Peer	76
Self	35
Undefined	31

**Job Title	Count**
PHP Developer	240
Software Test Engineer	36
Team Lead- SEO	34
SEO Executive	34
Team Lead - Asp.net	23
Sr. ASP.NET Developer	20
Sr. Web Designer	10
Project Coordinator	8
UI designer	6

**Scale Selected	Count**
Adequate	84
Sometimes Meets Expectations	70
Above adequate	43
Needs Improvement	42
Always Meets Expectations	40

4. **Visualizations**
The following visualizations were generated to highlight key trends and patterns within the data.

**Average Score by Job Title**: The bar chart shows the average score for each job title. The 
SEO Executive role has the highest average score, while Trainee Asp.net Developer has the lowest average score.
**Average Score by Evaluator**: This chart visualizes the average score given by each evaluator. It helps to identify any potential trends in how lenient or strict certain evaluators may be.
**Distribution of Evaluations by Level**: The bar chart provides a clear view of the number of evaluations for each level, confirming that Downward evaluations are the most frequent type in the dataset.
**Distribution of Performance Scores**: The histogram illustrates the frequency of different scores. It shows that scores are most concentrated between 6 and 8, indicating that a majority of performance ratings fall within this range.
