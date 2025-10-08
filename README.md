# Healthcare Data Analysis Project

**Healthcare Data Analysis Project** is a comprehensive data analysis tool designed to streamline data exploration, analysis, and visualisation. The tool supports multiple data formats and provides an intuitive interface for both novice and expert data scientists.

# ![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)

# Initial Setup
* This project is developed and tested with Python 3.12.10.
It is recommended to create a virtual environment before installing dependencies:

* Run the following in the terminal:  
```
    bash
    python3.12 -m venv .venv
    source .venv/Scripts/activate
    pip install -r requirements.txt
```

* The notebooks are designed to be ran and worked through in the following order:
1. 01_etl_pipeline
2. 02_basic_visualisations
3. 03_advanced_visualisations
4. [Healthcare Analysis Dashboard](https://public.tableau.com/app/profile/andrea.ferreira4559/viz/Healthcare-analysis-dashboard/MasterDashboardHealthcareCharges?publish=yes) created using Tableau

## Dataset Content
This project uses the [Healthcare Insurance Dataset](https://www.kaggle.com/datasets/willianoliveiragibin/healthcare-insurance) containing 1,337 records on how demographic and lifestyle factors influence medical insurance charges.

| Column        | Description                                                                                  |
|---------------|----------------------------------------------------------------------------------------------|
| age           | Age of the insured individual                                                                |
| sex           | Gender (male, female)                                                                        |
| bmi           | Body Mass Index — indicator of body fat based on height and weight                           |
| children      | Number of dependents covered by insurance                                                    |
| smoker        | Smoking status (yes/no)                                                                      |
| region        | Geographic region (northeast, northwest, southeast, southwest)                               |
| charges       | Individual medical insurance costs                                                           |


## Business Requirements

* Identify key factors that influence healthcare insurance charges.

* Compare costs across demographics including age, gender, and region.

* Determine the effect of lifestyle factors like BMI and smoking status on insurance charges.

* Provide visual insights to support decision-making for healthcare providers and policymakers.


## Hypothesis and how to validate?
* H1: Smokers will have higher insurance charges than non-smokers
* H2: Charges will be positively correlated with BMI
* H3: Charges will be positively correlated with age
* H4: There will be an effect of number of children on charges
* H5: There will be an effect of region on charges
* H6: There will be an effect of sex on charges  
  
Hypotheses will be validated through statistical tests and visualisations

## Project Plan
* Data Collection: Import dataset from Kaggle and validate contents.

* Data Cleaning: Handle missing values, standardize categories, and create BMI categories.

* Identify trends, distributions, and correlations.

* Visualization: Create charts and dashboards for insights using Python and Tableau.

* Interpretation & Reporting: Summarize insights, validate hypotheses, and document findings.

## The rationale to map the business requirements to the Data Visualisations
| Business Requirement                          | Visualisation Mapping                                    |
| --------------------------------------------- | -------------------------------------------------------- |
| Compare costs by smoker status                | Average Charges by Smoking Status (Bar Chart)            |
| Effect of age and BMI on charges              | Age vs Charges, BMI vs Charges (Scatter Plots)           |
| Regional disparities in charges               | Regional Cost Heatmap, Charges by Region & Smoker Status |
| Family impact (number of children) on charges | Average Charges by Number of Children (Bar Chart)        |
| Identify anomalies or outliers                | Outlier Detection: BMI vs Charges (Scatter Plot)         |


## Analysis techniques used
* Descriptive Statistics: Summary statistics to understand data distribution.

* Correlation Analysis: Explore relationships between numeric variables (age, BMI, charges).

* Visualisation: Bar charts, scatter plots, heatmaps, treemaps, dashboards.

* Limitations: Dataset size is small, no time-series data, and features are limited.

* Generative AI Tools were used for code optimization, visualization suggestions, and exploratory analysis guidance.

## Ethical considerations
* Dataset is anonymised and publicly available
* Analysis focuses on group-level insights, not individuals
* Results are for educational and analytical purposes only

## Dashboard Design
The [Healthcare Analysis Dashboard](https://public.tableau.com/app/profile/andrea.ferreira4559/viz/Healthcare-analysis-dashboard/MasterDashboardHealthcareCharges?publish=yes) is an interactive dashboard exploring healthcare charges across different demographics and regions. The goal is to uncover patterns and cost drivers in medical expenses using real world data.<br>

### Dashboard Design & Communication Strategy
**Project Title:** Healthcare Cost Analysis Dashboard  <br>

**1. Dashboard Pages and Content** <br>
This dashboard consists of a single interactive page designed to explore healthcare charges 
across demographics and regions. All visualizations are presented in floating mode for 
flexible layout and precise positioning.

**Content Blocks and Widgets** 
| Element                | Description                                                                                   |
|------------------------|-----------------------------------------------------------------------------------------------|
| Title Block            | Displays dashboard name and purpose at the top center                                         |
| Region Filter (Dropdown)| Floating filter widget allowing users to explore data by geographic region                   |
| Legend Blocks          | Floating legends for color-coded dimensions (e.g., Smoker status, Region)                     |
| Text Labels & Headers  | Section headers to group charts into themes (e.g., Lifestyle, Demographics)                   |


**Visualizations (7 Floating Charts)**
1. *Average Charges by Smoking Status* – Bar chart comparing costs between smokers 
and non-smokers 
2. *Average Charges by Number of Children* – Bar chart showing cost variation by family 
size 
3. *Age vs Charges* – Scatter plot revealing age-related cost trends 
4. *BMI vs Charges by Gender* – Scatter plot comparing BMI impact across genders 
5. *Regional Cost Heatmap* – Heatmap showing average charges by region 
6. *Charges by Region & Smoker Status* – Hierarchical view of cost drivers 
7. *Outlier Detection: BMI vs Charges* – Scatter plot identifying anomalies in cost vs BMI 

**2. Feature Revisions During Development** <br>
During development, several visual elements were revised to better communicate insights: 
- Replaced planned line chart with a scatter plot for Age vs Charges to better show 
individual variation 
- Switched from stacked bar chart to treemap for regional breakdown to highlight 
hierarchical relationships 
- Added outlier detection chart to surface anomalies in BMI vs Charges late in the 
process 

**3. Communicating Insights to Technical and Non-Technical Audiences**
**Design Strategies**
| Technique                | Purpose                                                                                   |
|--------------------------|-------------------------------------------------------------------------------------------|
| Clear Titles & Labels    | Help non-technical users understand chart purpose and axes                                |
| Interactive Filtering    | Region dropdown allows intuitive exploration of localized trends                          |
| Color Coding & Legends   | Visual cues for categories like smoker status and region                                  |
| Tooltips                 | Hover-over details for technical users without cluttering the layout                      |
| Chart Variety            | Mix of bar charts, scatter plots, heatmaps, and treemaps for accessibility               |
| Section Headers          | Thematic grouping to guide narrative flow for all audiences                               |

**4. Summary**<br>
This dashboard was designed to be both analytically powerful and visually intuitive, 
ensuring that stakeholders from all backgrounds can explore and understand the data. <br>It 
enables users to uncover cost drivers, identify regional disparities, and spot outliers — all 
through a clean, interactive interface. 

## Development Roadmap
* Learn advanced Tableau features and Python libraries (e.g., Plotly, Seaborn) to improve visualizations.

## Main Data Analysis Libraries
* Python libraries used:

pandas – data manipulation and CSV handling

numpy – numeric operations and calculations

matplotlib – static data visualizations

seaborn – advanced statistical visualizations

plotly – interactive visualizations

scipy – statistical tests

statsmodels – regression modeling and advanced stats

pingouin – additional statistical tests and normality checks

* Dashboard / BI Tools:

Tableau – for creating interactive dashboards

## Conclusions

* Smoking status, BMI, and age are major drivers of healthcare charges.

* Regional disparities and number of children have measurable effects on costs.


## Credits 

* Code Institute Learning Materials
* Generative AI (ChatGPT, CoPilot)
* Relevant Library Documentation (pandas, numpy, seaborn, matplotlib, plotly)
* Youtube Tutorials (Linked below)

### Content 

- Instructions on how to perform various tasks with Data Analysis Libraries referenced from Code Institute's Online Learning Platform.
- ChatGPT used to help plan project and brainstorm features.
- CoPilot used to help build and optimise code.
- Features from relevant library documentation used to create visualisations and customise them.
- [Tableau Basics for Beginner - Tableau in Two Minutes](https://www.youtube.com/watch?v=jEgVto5QME8)
- [Dashboard design guidance from Learn Tableau in Under 2 hours | Dashboards, Relationships, and Calculations](https://www.youtube.com/watch?v=TKG1_6lw1_c)

## Acknowledgements
* Thank you to James for helping to test the project.