# Analysis of Risk Factors for Cardiovascular Diseases

This project aims to analyse how key factors, such as lifestyle choices or medical indicators, may affect the likelihood of developing cardiovascular diseases (CVD).

# ![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)


## Dataset Content
- Data source: https://data.world/kudem/heart-disease-dataset
- Data author: [Kuzak Dempsy](https://data.world/kudem)
- Kaggle download link: https://www.kaggle.com/datasets/thedevastator/exploring-risk-factors-for-cardiovascular-diseas 

|Name of feature|Description|Data type|
| ----------- | ----------- | ----------- |
|`index`|Index of the entry|Integer|
|`id`|Unique identifier assigned to each person|Integer|
|`age`|Age of the person in days|Integer|
|`gender`|Gender of the person, 1 = male, 2 = female|Integer|
|`height`|Height of the person in cm|Integer|
|`weight`|Weight of the person in kg|Float|
|`ap_hi`|Systolic blood pressure reading|Integer|
|`ap_lo`|Diastolic blood pressure reading|Integer|
|`cholesterol`|Cholesterol level|Integer|
|`gluc`|Glucose level|Integer|
|`smoke`|Smoking status, 0 = non smoker, 1 = smoker|Integer|
|`alco`|Alcohol status, 0 = do not consume alcohol, 1 = consume alcohol|Integer|
|`active`|Physical activity status, 0 = non active, 1= active|Integer|
|`cardio`|Presence of cardiovascular disease, 0 = non present, 1 = present|Integer|


## Business Requirements
* Identify key factors contributing to the development of CVD
* Generate Key insights on how different medical indicators and lifestyle choices may influence the development of CVD
* Create a machine learning model that will predict the likelihood of an individual having CVD based on various factors
* Present findings to a non techical audience through a dashboard


## Hypothesis and how to validate?
- Older individuals are more likely to develope cardiovascular disease (CVD)
- Males are more likely to develope CVD than females
- High blood pressure increase the likelihood of developing CDV
- High cholesterol individuals are more likely to have CDV
- Physically active individuals are less likely to have CDV
- Smokers are more likely to have CDV
- Alcohol consumption increase the likelyhood of developing CDV

Relevent statistical tests will be conducted during the EDA process. Visualisations will also be provided to support any conclusions drawn.

## Project Plan
### **Overview**
1. **Extract Transform Load (ETL):**  
Conducted basic cleaning of the dataset, detecting and handling missing or duplicate data. Removing obvious errors and unnecessary features.
2. **Exploratory Data Analysis (EDA): Feature Engineering and Descriptive Analysis**  
- Categorical data values represented by integers were replaced to actural categorical values for easier interpritation
- New features added through manipulation of existing data
- Extreme outliers were detected and handled
- Descriptive analysis was conducted to get an overview of the data after transforming
3. **EDA: Hypothesis Testing and Visualisation**
Hypotheses were tested using statistical tests such as the chi squred test or the Mann-Whitney test to prove initial hypotheses and visualisation were produced using matplotlib and seaborn to support conclusions.
4. **Machine Learning:**  
Trained Logistic Regression and Random Forest models to predict CVD, using an 80/20 train-test split and ROC-AUC for evaluation.
5. **Dashboarding**
A PowerBI dashboard was created to present the data and insights to a non technical audience.

## The rationale to map the business requirements to the Data Visualisations
* Statistical tests provided interpretations of the relationships between risk factors and CVD.
* Conclusions were confirmed and checked using visualisations.
* Machine learning models validated and extended these findings through predictive analysis.
* Findings and insights are presented to a non technical audience through a dashboard.


## Analysis techniques used

- **Descriptive statistics:** Summarised data distributions.  
- **Normality testing (Shapiro–Wilk):** Checked assumptions.  
- **Non-parametric tests (Mann–Whitney U, Chi-Square):** Assessed group differences and associations.  
- **Machine learning (Logistic Regression, Random Forest):** Predicted CVD and identified key features.

### Limitations & Alternatives
- Limited lifestyle and family history data reduced model accuracy.
- Source of the Dataset contains some vague descriptions of the features. For example, levels of cholesterol.
- Non-normal distributions required non-parametric tests.
- Some bias and skew in the sample.
- Future work could include more informative features.

## Ethical considerations
* No identifiable features for individuals in the dataset.
* Individuals with certain medical conditions such as restricted growth may be represented inaccurately.
* Demographic of the dataset is limited and may not accurately portray populations of different parts of the world.

## Dashboard Design
The dashboard was designed with two interactive pages to explore and communicate insights about cardiovascular disease (CVD) risk factors. It allows users to interactively filter, compare, and interpret patterns in the dataset through clear and intuitive visuals.

The dashboard was built to:
- Provide a balanced view of both numerical and categorical risk factors.  
- Use interactive filters and slicers to promote exploratory analysis without coding.  
- Ensure accessibility and interpretability for both health data professionals and general stakeholders.  
- Communicate complex statistical insights through visual summaries, allowing users to connect data patterns to real-world health implications.


## Unfixed Bugs
* No known unresolved issues

## Development Roadmap

- A significant amount of time was spent on the **Exploratory Data Analysis (EDA)** phase due to uncertainty in the notebook’s structure, resulting in frequent revisions and backtracking.  
- Future projects would benefit from establishing a **clear project methodology and workflow** at the start to improve efficiency and maintain focus.  

For future project:
- Seek to use **Streamlit** to develop an interactive and shareable dashboard interface.  
- Seek to implement **Heroku (or similar cloud platforms)** for model and dashboard deployment to allow easy public access and demonstration.  



## Main Data Analysis Libraries
* **numpy:** Used for fast numerical computations and handling arrays for mathematical operations.
* **pandas:** Managed, cleaned, and transformed tabular data efficiently using DataFrames.
* **matplotlib:** Created static visualisations such as histograms, bar charts, and box plots for EDA.
* **seaborn:** Produced enhanced statistical visualisations with simpler syntax and built-in styling.
* **plotly:** Built interactive and dynamic charts for dashboard integration and data exploration.
* **scipy:** Used to perform statistical hypothesis tests such as Shapiro–Wilk, Mann–Whitney U, and Chi-Square tests.
* **scikit-learn:** Implemented machine learning models, preprocessing pipelines, and model evaluation metrics.




## Credits 
- Data source: https://data.world/kudem/heart-disease-dataset
- Data author: [Kuzak Dempsy](https://data.world/kudem)
- Generative AI such as Copilot and ChatGPT were used to assist with ideation and code optimisation
- Code institute logo [link](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)



## Acknowledgements
Many thanks to Vasi, my fellow cohorts and the team at Code Institute who provided support through out this project.