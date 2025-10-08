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
| bmi_category  | BMI category: Underweight (<18.5), Normal (18.5–24.9), Overweight (25–29.9), Obese (≥30)     |


## Business Requirements
* Describe your business requirements


## Hypothesis and how to validate?
* H1: Smokers will have higher insurance charges than non-smokers
* H2: Charges will be positively correlated with BMI
* H3: Charges will be positively correlated with age
* H4: There will be an effect of number of children on charges
* H5: There will be an effect of region on charges
* H6: There will be an effect of sex on charges  
  
Hypotheses will be validated through statistical tests and visualisations

## Project Plan
* Outline the high-level steps taken for the analysis.
* How was the data managed throughout the collection, processing, analysis and interpretation steps?
* Why did you choose the research methodologies you used?

## The rationale to map the business requirements to the Data Visualisations
* List your business requirements and a rationale to map them to the Data Visualisations

## Analysis techniques used
* List the data analysis methods used and explain limitations or alternative approaches.
* How did you structure the data analysis techniques. Justify your response.
* Did the data limit you, and did you use an alternative approach to meet these challenges?
* How did you use generative AI tools to help with ideation, design thinking and code optimisation?

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

## Unfixed Bugs
* Please mention unfixed bugs and why they were not fixed. This section should include shortcomings of the frameworks or technologies used. Although time can be a significant variable to consider, paucity of time and difficulty understanding implementation are not valid reasons to leave bugs unfixed.
* Did you recognise gaps in your knowledge, and how did you address them?
* If applicable, include evidence of feedback received (from peers or instructors) and how it improved your approach or understanding.

## Development Roadmap
* What challenges did you face, and what strategies were used to overcome these challenges?
* What new skills or tools do you plan to learn next based on your project experience? 

## Main Data Analysis Libraries
* Here you should list the libraries you used in the project and provide an example(s) of how you used these libraries.

## Conclusions

## Credits 

* In this section, you need to reference where you got your content, media and extra help from. It is common practice to use code from other repositories and tutorials, however, it is important to be very specific about these sources to avoid plagiarism. 
* You can break the credits section up into Content and Media, depending on what you have included in your project. 

### Content 

- The text for the Home page was taken from Wikipedia Article A
- Instructions on how to implement form validation on the Sign-Up page was taken from [Specific YouTube Tutorial](https://www.youtube.com/)
- The icons in the footer were taken from [Font Awesome](https://fontawesome.com/)

### Media

- The photos used on the home and sign-up page are from This Open-Source site
- The images used for the gallery page were taken from this other open-source site



## Acknowledgements (optional)
* Thank the people who provided support through this project.
