
- Revision on python 
- after this we try out on provided dataset 
- Review the instruction to do on these dataset
- Final : Visualize the instruction 



Deadline: Tuesday



our first project : 


### **Phase 1: Data Exploration & Cleaning**

1. Load dataset and understand structure
    
2. Handle missing values
    
3. Verify data types and basic statistics
    

### **Phase 2: Core Analysis**

**Income Disparity Analysis:**

- Compare average water access across income groups (High/Upper middle/Lower middle/Low)
    
- Visualize with bar charts
    

**Country Performance Ranking:**

- Identify top 10 and bottom 10 countries for water access
    
- Analyze income patterns among best/worst performers
    

**Urban-Rural Divide:**

- Calculate urban-rural access gaps
    
- Find countries with largest inequalities
    

**Population Impact:**

- Create scatter plot: Population vs Water Access
    
- Identify outliers (large populations with good access, small populations with poor access)
    

### **Phase 3: Key Insights**

Answer these specific questions:

1. **The Rich-Poor Water Gap:** What's the percentage difference in water access between high-income and low-income countries?
    
2. **Urban-Rural Inequality:** Which 3 countries have the largest urban-rural gaps, and how big are these gaps?
    
3. **Population Paradox:** Find one small country with surprisingly poor access and one large country with surprisingly good access.
    

## **Expected Deliverables**

- 4 visualizations (income comparison, rankings, urban-rural gaps, population scatter plot)



## Day 1: Data Acquisition and Cleaning Mastery

**Goal:** Master data preparation, which is the most time-consuming and critical part of analysis.

- **Task 1.1: Ingestion and Initial Assessment (3 hours)**
    
    - Load the data into a suitable tool (Python with Pandas or R).
        
    - **Inspect and document:** Identify the unique countries/areas, the range of years, and the total number of unique indicators (columns) present.
        
    - **Initial data types:** Check the data types of all columns and correct them (e.g., ensure numeric values aren't stored as strings).
        
- **Task 1.2: Missing Value and Duplication Handling (4 hours)**
    
    - **Missingness analysis:** Calculate the percentage of missing values (`NaN` or similar) for _every_ column.
        
    - **Strategy development:** Decide on a strategy for columns with high missingness. Drop columns with greater than 75% missing data.
        
    - **Imputation:** For key columns with low missingness (e.g., under 10%), use appropriate imputation techniques like forward-fill, mean/median imputation, or interpolation. **Document your choices.**
        
    - **Duplicate check:** Identify and remove any fully duplicated rows.
        
- **Task 1.3: Data Transformation and Feature Engineering (2 hours)**
    
    - **Standardize Country Names:** Clean and standardize country/area names to ensure consistency.
        
    - **Create a Composite Index:** Select 2-3 related columns (e.g., GDP per capita, Life Expectancy, Education Index) and combine them into a single, simple **"Development Score"** using a weighted average or min-max scaling to practice feature engineering.
        

---

## Day 2: Exploratory Data Analysis (EDA) and Visualization

**Goal:** Use statistics and visualizations to find patterns, anomalies, and relationships.

- **Task 2.1: Univariate and Descriptive Analysis (3 hours)**
    
    - For 5-7 key indicators (e.g., Total Population, Infant Mortality Rate, CO2 Emissions), calculate **summary statistics** (mean, median, standard deviation, min, max, quartiles).
        
    - **Visualize distributions:** Use **histograms** or **Box Plots** for these key indicators to understand their shape and identify outliers.
        
- **Task 2.2: Bivariate Analysis and Correlation (4 hours)**
    
    - **Correlation Matrix:** Compute a correlation matrix for all numeric columns.
        
    - **Deep Dive:** Focus on the strongest and weakest correlations. Create **scatter plots** between your newly created "Development Score" and key indicators like fertility rate or poverty level.
        
    - **Time Series Plotting:** For 3-5 major global regions (e.g., Asia, Africa, Europe), plot the trend of a single key indicator (e.g., Population Growth Rate) over the entire time span of the dataset to analyze change over time.
        
- **Task 2.3: Geographical Analysis (2 hours)**
    
    - **Ranking:** Create a table that ranks the top 10 and bottom 10 countries based on your "Development Score" for the most recent available year.
        
    - **Visual Map:** If possible, use a library (like Plotly or Folium) to create a basic **Choropleth map** showing the distribution of one variable (e.g., Life Expectancy) across the world.
        

---

## Day 3: Insight Generation and Presentation

**Goal:** Consolidate findings and structure them into a narrative, mimicking a real-world report.

- **Task 3.1: Hypothesis Testing and Group Comparison (4 hours)**
    
    - **Group Segmentation:** Divide the countries into two or three meaningful groups based on a key metric (e.g., "High Income," "Middle Income," "Low Income" or by continent).
        
    - **Statistical Comparison:** Perform a basic **t-test or ANOVA** (if you're familiar with them) to determine if the _means_ of a key indicator (like Infant Mortality) are significantly different between the country groups you created.
        
    - **Justify and explain** the real-world implications of any statistical difference you find.
        
- **Task 3.2: Final Visualizations for Storytelling (3 hours)**
    
    - Refine the best 4-5 visualizations from Day 2 into **publication-ready quality**. Ensure they have clear titles, axis labels, and a caption explaining the key takeaway.
        
    - Focus on telling a story, such as "The relationship between wealth (GDP) and health (Life Expectancy) has changed over the last 20 years."
        
- **Task 3.3: Executive Summary and Next Steps (2 hours)**
    
    - Write a **brief, three-paragraph executive summary** of your analysis.
        
        1. **Paragraph 1:** What was the goal and what data did you use?
            
        2. **Paragraph 2:** What were the two most significant insights (e.g., the trend for a specific region, or a strong correlation)?
            
        3. **Paragraph 3:** What are the limitations of the data (e.g., missing data, data definitions) and what would be the next step for a deeper analysis (e.g., building a predictive model)?