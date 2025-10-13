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

### **Limitations & Alternatives**
- Limited lifestyle and family history data reduced model accuracy.
- Non-normal distributions required non-parametric tests.
- Future work could include more informative features.

## Ethical considerations
* Source of the Dataset contains some vague descriptions of the features. For example, levels of cholesterol.
* Individuals with certain medical conditions such as restricted growth may be represented inaccurately.
* Demographic of the dataset is limited and may not accurately portray populations of different parts of the world.

## Dashboard Design
* List all dashboard pages and their content, either blocks of information or widgets, like buttons, checkboxes, images, or any other item that your dashboard library supports.
* Later, during the project development, you may revisit your dashboard plan to update a given feature (for example, at the beginning of the project you were confident you would use a given plot to display an insight but subsequently you used another plot type).
* How were data insights communicated to technical and non-technical audiences?
* Explain how the dashboard was designed to communicate complex data insights to different audiences. 

## Unfixed Bugs
* Please mention unfixed bugs and why they were not fixed. This section should include shortcomings of the frameworks or technologies used. Although time can be a significant variable to consider, paucity of time and difficulty understanding implementation are not valid reasons to leave bugs unfixed.
* Did you recognise gaps in your knowledge, and how did you address them?
* If applicable, include evidence of feedback received (from peers or instructors) and how it improved your approach or understanding.

## Development Roadmap
* What challenges did you face, and what strategies were used to overcome these challenges?
* What new skills or tools do you plan to learn next based on your project experience? 


## Main Data Analysis Libraries
* numpy:
* pandas:
* matplotlib:
* seaborn:
* plotly:
* scikit-learn:



## Credits 

- Data source: https://data.world/kudem/heart-disease-dataset

### Content 

- Generative AI such as Copilot and ChatGPT were used to assist with ideation and code optimisation

### Media

- The photos used on the home and sign-up page are from This Open-Source site
- The images used for the gallery page were taken from this other open-source site



## Acknowledgements (optional)
* Thank the Vasi and Niel who provided support through out this project.