# Wildfire-Analysis : Data-Capstone-Project

## Project Description
This data science capstone project analyzes historical wildfire data from 1992 to 2020 across the United States. The primary focus is to identify patterns, understand the main causes of wildfires, and develop data-driven recommendations for prevention and resource allocation strategies. By examining decades of wildfire incidents, this analysis aims to provide actionable insights that can help reduce wildfire occurrences and improve response effectiveness.

## Objective
In this project, my primary focus is on understanding wildfire patterns and identifying key factors that contribute to wildfire incidents in the USA. To achieve this goal efficiently, the project has been divided into several objectives:

1. **Temporal Pattern Analysis**: Examine wildfire trends over the 28-year period (1992-2020) to identify seasonal patterns, yearly trends, and long-term changes in wildfire frequency and severity.

2. **Geographic Distribution**: Analyze the spatial distribution of wildfires across different states and regions to identify high-risk areas and understand regional variations.

3. **Cause Analysis**: Identify and categorize the primary causes of wildfires (natural vs. human-caused) and determine which factors contribute most significantly to wildfire incidents.

4. **Severity Assessment**: Evaluate wildfire severity metrics including acres burned, duration, and containment challenges to understand the impact and scale of different wildfire events.

5. **Predictive Insights**: Develop insights that can inform prevention strategies and resource allocation for wildfire management.

## Data Overview

The dataset represents wildfire incidents across the United States from 1992 to 2020. After examining the data fields, the dataset generally provides the following key information:

### Fire Incident Details:
- **Fire Identification**: Unique identifiers for each wildfire incident
- **Temporal Information**: Discovery date, containment date, fire year, fire season
- **Geographic Information**: State, county, latitude, longitude coordinates
- **Fire Characteristics**: Fire size (acres), fire cause, fire type

### Key Data Dimensions:
- **Time Period**: 28 years (1992-2020)
- **Geographic Coverage**: All 50 US states
- **Incident Count**: [Insert total number of wildfire incidents analyzed]
- **Cause Categories**: Lightning, human activity, equipment use, arson, debris burning, and others

## Technologies Used

- **Python 3.x**: Primary programming language
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computations
- **Matplotlib & Seaborn**: Static data visualizations
- **Plotly**: Interactive visualizations
- **Jupyter Notebook**: Analysis documentation and presentation

## METHODOLOGY

### Business Demand Analysis

**Requirements**: Create comprehensive analysis and visualizations to understand wildfire patterns, identify primary causes, and propose prevention strategies to reduce wildfire incidents across the USA.

**Method**: Descriptive analysis, exploratory data analysis (EDA), statistical analysis, and geospatial analysis

**Tools Used**:
- Python (Data preprocessing, data cleaning, EDA, statistical analysis, visualization)
- Libraries: Pandas, NumPy, Matplotlib, Seaborn, Plotly (for interactive visualizations)
- Jupyter Notebook for analysis documentation

**Data Source**: Fire Program Analysis (FPA) Database, 1992-2020
**Analysis Period**: 28 years covering 1.88 million geo-referenced wildfire records
**Primary Focus States**: California, Georgia, and Texas (highest fire intensity states)
**Best Predictive Model**: Random Forest with hyperparameter tuning (79.92% accuracy)

### Analysis Components:

#### 1. Temporal Analysis Dashboard
- Yearly wildfire trends (1992-2020)
- Seasonal patterns and peak wildfire months
- Long-term trend analysis
- Fire frequency over time

#### 2. Geographic Distribution Analysis
- State-by-state wildfire frequency
- Regional hotspot identification
- Geographic clustering of high-risk areas
- Spatial distribution patterns

#### 3. Cause Investigation
- Classification of wildfire causes (lightning, human activity, equipment, arson, etc.)
- Percentage breakdown by cause category
- Cause variation by region and season
- Human-caused vs. natural wildfire comparison

#### 4. Severity & Impact Analysis
- Total acres burned analysis
- Average fire size by cause and region
- Duration and containment time analysis
- Economic and environmental impact assessment

#### 5. Prevention Recommendations
- Data-driven prevention strategies
- Resource allocation recommendations
- High-risk area identification
- Seasonal preparedness guidelines

## Data Pre-Processing & Data Cleaning

The data pre-processing and data cleaning were performed using Python.

**Detailed Notebook**: [here](https://github.com/poojapatel26/Wildfire-Analysis---Data-Capstone-Project/blob/main/Wildfire_Analysis_Final_Project.ipynb%20-%20Colaboratory.pdf)

### Data Cleaning Steps:
1. **Handling Missing Values**: Identified and handled missing data in key columns such as fire cause, location, and severity metrics
2. **Date Formatting**: Standardized date formats for temporal analysis
3. **Geographic Data Validation**: Verified state/county information and corrected inconsistencies
4. **Outlier Detection**: Identified and analyzed extreme values in acres burned and fire duration
5. **Data Type Conversion**: Converted data types for efficient analysis
6. **Feature Engineering**: Created additional features such as fire season, decade classification, and severity categories




## Key Insights

### 1. Temporal Patterns:

#### Yearly Trend Analysis
- **Peak Wildfire Years**: The analysis covers the period from 1992 to 2020, with data showing consistent wildfire activity throughout this 28-year period
- **Increasing/Decreasing Trends**: The dataset demonstrates ongoing wildfire challenges across the United States, with human-caused fires dominating throughout the study period
- **Recent Decade Comparison**: Analysis shows that wildfires remain a persistent threat, with human activities being the primary driver of fire incidents across all time periods analyzed

#### Seasonal Patterns
- **Peak Fire Season**: Late spring to summer (May through July are the peak months)
- **Off-Season Activity**: December and November show the lowest wildfire activity, with gradually increasing activity from January through April
- **Climate Correlation**: Higher temperatures and drier conditions during late spring and summer make it easier for fires to start and spread. Additionally, increased outdoor recreational activities during these warmer months contribute to more accidental fires from campfires, equipment/vehicle use, and debris burning

### 2. Geographic Distribution:

#### Highest Risk States
- **Top 3 States by Fire Frequency**: 
  1. California (251,880 fire intensity)
  2. Georgia (185,040 fire intensity)
  3. Texas (180,080 fire intensity)
- **Top 5 States by Fire Frequency**: California, Georgia, Texas, North Carolina, and Florida
- **Regional Patterns**: Six out of the top 10 most fire-prone states are from southeastern states. The analysis reveals distinct regional vulnerabilities, with the West Coast (California) and Southeast (Georgia, Texas, and surrounding states) experiencing the highest wildfire intensity

#### Geographic Hotspots
- **California, Texas, and Georgia** stand out as the three states with the most significant wildfire impact and were selected for detailed analysis
- The **southeastern United States** shows particularly high fire frequency, with 6 of the top 10 fire-prone states located in this region
- The most fire-prone jurisdictions include **District of Columbia (DC), Delaware (DE), and Vermont (VT)** when considering fire density relative to land area

### 3. Cause Analysis:

#### Primary Causes Breakdown
Based on the analysis of California, Texas, and Georgia (the most impacted states):

- **Natural Causes (Lightning)**: Approximately 10-15% of total wildfires
- **Human-Caused Fires**: Approximately 85-90% of total wildfires

**Top 3 Most Frequent Human-Caused Fires:**
  1. **Debris/Open Burning**: Most frequent cause (vegetation, dead plants, and organic materials on forest floors act as fuel)
  2. **Equipment/Vehicle Use**: Second most frequent cause
  3. **Arson**: Third most frequent cause

**Other Human Activities Include:**
  - Recreation/Ceremony (campfires and cultural/religious ceremonies)
  - Electrical utility (power lines)
  - Fireworks
  - Railroad operations
  - Smoking
  - Fire by a minor

#### Cause by Region
- **Across all three most-impacted states (CA, TX, and GA)**, human activity is the main contributing factor to wildfires
- **California** shows particularly high incidents of debris/open burning
- **Georgia** demonstrates significant debris burning-related fires
- The pattern is consistent: human-caused fires (especially accidental ones from debris burning and equipment use) far outnumber natural causes across all high-risk regions

### 4. Severity Analysis:

#### Fire Size Distribution
Based on average fire sizes by cause (in acres):

- **Largest Fires** caused by:
  1. Firearms & Explosives: ~370 acres average
  2. Natural causes (Lightning): ~210 acres average
  3. Electrical Utility: ~160 acres average
  
- **Medium-Large Fires**:
  - Recreation/Ceremony: ~70 acres average
  - Fireworks: ~60 acres average
  
- **Smaller Fires**:
  - Equipment/Vehicle Use: ~45 acres average
  - Arson: ~35 acres average
  - Railroad Operations: ~25 acres average
  - Smoking: ~20 acres average
  - Fire by a Minor: ~10 acres average
  - Debris/Open Burning: ~5 acres average

#### Impact Assessment
- **Total Wildfires Analyzed**: 1.88 million geo-referenced wildfire records
- **Study Period**: 28 years (1992-2020)
- **Most Impacted States**: California leads with 251,880 fire intensity, followed by Georgia (185,040) and Texas (180,080)
- **Largest Fire Causes**: Firearms & Explosives and Natural causes (lightning) produce the largest average fire sizes, though they occur less frequently than other causes
- **Most Destructive Pattern**: While debris burning is the most frequent cause, fires from firearms/explosives and electrical utilities result in significantly larger burned areas

### 5. Prevention Opportunities:

#### High-Priority Focus Areas

**Top Preventable Causes (in order of frequency):**
1. **Debris/Open Burning** - Most frequent human-caused wildfire trigger
2. **Equipment/Vehicle Use** - Second most frequent cause
3. **Arson** - Third most frequent cause

**Geographic Areas Needing Most Attention:**
- **Priority 1**: California (highest fire intensity at 251.88k)
- **Priority 2**: Georgia (185.04k fire intensity)
- **Priority 3**: Texas (180.08k fire intensity)
- **Additional Focus**: Southeastern states showing high fire frequency

**Seasonal Preparedness Needs:**
- **Critical Period**: Late spring through summer (May-July peak months)
- **Pre-season Preparation**: April requires enhanced readiness as activity increases
- **Year-round**: December-March require baseline monitoring with preparations beginning in February

**Infrastructure Vulnerabilities:**
- Electrical utility infrastructure (power lines) requires attention despite lower frequency, as these fires average 160 acres and cause significant damage


## Suggestions

### 1. Prevention Strategies

**Target Human-Caused Fires**: Since approximately **85-90%** of wildfires are caused by human activities, implement comprehensive prevention programs:

- **Public Education Campaigns**: Launch targeted awareness campaigns during peak fire seasons (May-July) about safe practices for:
  - **Debris burning management** (the #1 cause): Proper timing, clearing zones, and monitoring
  - **Equipment and vehicle use**: Spark arrestors, avoiding dry vegetation, proper maintenance
  - **Campfire safety**: Complete extinguishment, proper locations, water availability
  
- **Stricter Regulations**: 
  - Enforce burn bans during high-risk periods (late spring to summer)
  - Implement penalty systems for negligent fire-starting behaviors
  - Require permits for debris burning with strict weather and timing conditions
  - Mandate equipment safety standards for vehicles and machinery in wildfire-prone areas
  
- **Community Engagement**: 
  - Develop community-based fire prevention programs in California, Georgia, and Texas
  - Partner with local organizations for grassroots education
  - Create neighborhood fire watch programs

### 2. Resource Allocation & Preparedness

**Geographic Priority**: Focus resources on high-risk states and regions identified in the analysis:

- **Pre-positioning Resources**: Deploy firefighting resources to California, Georgia, and Texas before peak fire season (by late April)
- **Regional Task Forces**: Establish specialized wildfire response teams in the top 10 fire-prone states, with emphasis on southeastern states
- **Early Warning Systems**: Implement advanced monitoring systems in identified high-risk zones, particularly in California and the Southeast

**Seasonal Readiness**:
- **Peak Season Preparation**: Increase staffing and equipment readiness from May through July
- **Pre-Season Ramp-up**: Begin enhanced preparations in April as wildfire activity increases
- **Year-Round Monitoring**: Maintain baseline monitoring capabilities during December-March off-peak months
- **Climate-Adaptive Planning**: Adjust resource allocation based on drought conditions and climate forecasts, particularly monitoring spring drought conditions that can extend fire seasons

### 3. Infrastructure & Technology Investment

**Detection & Response**:
- **Early Detection Systems**: Invest in satellite monitoring, drone surveillance, and AI-powered fire detection in California, Georgia, Texas, and other high-risk areas
- **Rapid Response Protocols**: Develop faster initial attack capabilities to contain fires while they're still small, particularly important for debris burning fires
- **Communication Networks**: Establish robust communication infrastructure for coordinated wildfire response

**Electrical Infrastructure Upgrades**:
- **Priority Investment**: Check and replace defective electrical utility infrastructure like power lines
- **Justification**: While electrical utility fires are less frequent, they contribute to the third-largest average fire size (~160 acres) and cause significant damage
- **Action Items**: Enhance and upgrade electrical utility systems in high-risk areas to reduce wildfire severity

### 4. Data-Driven Policy Making

**Evidence-Based Regulations**:
- Use this analysis to inform policy decisions about land management, building codes in wildfire-prone areas, and vegetation management
- **Risk Mapping**: Develop and regularly update wildfire risk maps for public use and development planning, with special focus on the peak fire months (May-July)
- **Insurance & Zoning**: Inform insurance risk assessments and zoning decisions with comprehensive wildfire data, particularly for California, Georgia, and Texas

**Seasonal Restrictions**:
- Implement stronger seasonal restrictions on debris burning during peak months
- Create graduated restriction levels based on real-time fire danger assessments
- Coordinate burn permits with weather forecasting

### 5. Research & Continuous Improvement

**Ongoing Analysis**:
- Continue tracking wildfire patterns to identify emerging trends
- Study the effectiveness of implemented prevention strategies
- Analyze climate change impacts on wildfire frequency and severity
- Research innovative suppression technologies and techniques

**Model Improvement**:
- Enhance machine learning models to better predict "Arson" and "Other" categories (currently at 31% and 11% accuracy respectively)
- Incorporate additional environmental variables (humidity, wind patterns, drought indices)
- Develop real-time prediction capabilities using Flask or Streamlit deployment

### 6. Interagency Collaboration

**Coordinated Approach**:
- Strengthen collaboration between federal, state, and local fire management agencies, particularly in high-risk states
- Share data and best practices across jurisdictions
- Develop unified response protocols for large-scale wildfire events
- Create cross-border coordination mechanisms for fires that span multiple states, especially important in the Southeast where multiple high-risk states are adjacent

**Multi-State Initiatives**:
- Establish a California-Georgia-Texas wildfire prevention coalition given their status as the three most-impacted states
- Create regional Southeast wildfire prevention network
- Share resources and personnel during peak season across state lines

---

**Data Source**: Fire Program Analysis (FPA) Database, 1992-2020
**Analysis Period**: 28 years covering 1.88 million geo-referenced wildfire records
**Primary Focus States**: California, Georgia, and Texas (highest fire intensity states)
**Best Predictive Model**: Random Forest with hyperparameter tuning (79.92% accuracy)


## Project Structure

```
Wildfire-Analysis-Data-Capstone-Project/
│
├── Wildfire_Analysis_Final_Project.ipynb    # Main analysis notebook
├── Analysis_Results.pdf                      # Detailed findings document
├── Final_Poster (1).jpg                      # Poster 
├── README.md                                 # Project documentation
```

## Key Deliverables

1. **Comprehensive Analysis Notebook**: Complete Python analysis with visualizations and statistical insights
2. **Results Document**: Detailed PDF report of findings and recommendations
3. **Project Poster**: Visual summary of methodology, key findings, and recommendations
4. **README Documentation**: Project overview and methodology guide

## Future Enhancements

- **Predictive Modeling**: Develop machine learning models to predict wildfire risk based on weather, vegetation, and historical patterns
- **Real-Time Dashboard**: Create an interactive dashboard for real-time wildfire monitoring and risk assessment
- **Economic Impact Analysis**: Quantify the economic costs of wildfires and ROI of prevention strategies
- **Climate Integration**: Incorporate climate change projections into long-term wildfire risk forecasting


## Acknowledgments

This project was completed as part of a Data Science Capstone program, analyzing publicly available wildfire data to contribute to wildfire prevention and management strategies in the United States.



