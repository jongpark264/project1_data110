# project_1_data110
This project explores a dataset using basic data visualization techniques.

# 📊 Dataset
This project analyzes the relationship between public safety and city administrative actions using two datasets from Baltimore City Open Data:
1. Baltimore Towing Data: Contains records of towed vehicles, including locations, pickup types, "Stolen Vehicle" flags, and the total amount paid for retrieval.
2. BPD Arrests Data: Provides information on arrests, including the police district, the age of the individual, and the type of charges.
3. Key Variables: Police District (9 sectors), Total Paid Amount, Average Offender Age, and Stolen Vehicle Rate.

🔍 What I Did
1. I focused on establishing a high-integrity dataset and exploring the relationships between administrative actions and criminal demographics through the following steps:
  - Advanced Data Mapping & Refinement Initial Standardization: Re-standardized the inconsistent address system of the Towing dataset to match the Baltimore Police Department (BPD) district criteria.
  - Multi-Stage Processing: Performed an initial geographic distribution using Mapline, followed by training an AI model to recognize and categorize complex address patterns.
  - Iterative Verification: Conducted 15 cycles of district assignment and rigorous verification.
    a. Performed random sampling in each district to verify spatial accuracy.
    b. Conducted ZIPCODE consistency checks to ensure geographic alignment.
  - Mapping Success: Successfully mapped 38,030 data points out of a total of 38,176 (excluding 146 addresses), achieving a 99.62% success rate.
2. Spatial Grid Visualization
  - Designed a 3x3 geographic grid layout to represent the 9 Baltimore districts according to their actual cardinal directions.
  - Visualized the intersection of arrest density and towing frequency within this grid.
3. Statistical Modeling (Linear Regression)
  - Developed a Linear Regression model to explore the correlation between the average age of offenders and the rate of stolen vehicle recoveries across districts.
  - Analyzed the statistical significance of demographic trends in relation to specific crime types.
4. Economic Distribution Analysis
  - Used Boxplots to analyze the distribution, medians, and outliers of vehicle retrieval costs (Total Paid) across different districts to identify economic disparities.

# 🛠 Tools Used
- Programming Language: R
- Libraries: tidyverse (dplyr for data manipulation, ggplot2 for visualization)
- Preprocessing Tools: MApline, Gemini, Grok.

## 📌 Author
  Jong-Geon Park
