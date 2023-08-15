# Exploring Organ, Eye, and Tissue Donations - Python Analysis
### SUMMARY: 
A project using Jupyter Notebooks to clean, merge, analyze and finally visualize publicly available data from the Organ Procurement & Transplantation Network (OPTN) and the U.S. Census Bureau.  

### OBJECTIVES
• Clean and merge four data sets: living donors (2013-2022), deceased donors (2013-2022), census data (2010-2019), and census data (2022-2022). 

• Analyze the data to uncover any potential differences based on state, gender, age-grouping, ethnicity or donor type.

• Use machine learning (linear regression and K-means clustering) to investigate whether the rates of donation for living and deceased donors are related.

• Create a Tableau dashboard that gives others an overview of the analysis completed during this project and allows others to explore the data further.

### DATA
Organ donor data retrieved from the Organ Procurement & Transplant Network on May 25, 2023 via  https://optn.transplant.hrsa.gov/data/view-data-reports/build-advanced/ 
NOTE: The collection of the OPTN data was supported in part by Health Resources and Services Administration contract HHSH250-2019-00001C. The content is the responsibility of the authors alone and does not necessarily reflect the views or policies of the Department of Health and Human Services, nor does mention of trade names, commercial products, or organizations imply endorsement by the U.S. Government.

Population data retrieved from the U.S. Census Bureau via two data sets on July 3, 2023:
"Annual State Resident Population Estimates for 6 Race Groups (5 Race Alone Groups and Two or More Races) by Age, Sex, and Hispanic Origin: April 1, 2010 to July 1, 2019 [<1.0 MB]" https://www2.census.gov/programs-surveys/popest/tables/2010-2019/state/asrh/sc-est2019-alldata6.csv 
"Annual State Resident Population Estimates for 6 Race Groups (5 Race Alone Groups and Two or More Races) by Age, Sex, and Hispanic Origin: April 1, 2020 to July 1, 2022 (SC-EST2022-ALLDATA6) [< 1.0 MB]" https://www2.census.gov/programs-surveys/popest/datasets/2020-2022/state/asrh/sc-est2022-alldata6.csv 


### TOOLS
*Language:* Python

*Libraries:* Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn

*Software:* Jupyter Notebooks and Excel


### SKILLS DEMONSTRATED

• **Cleaning data:**  resolved missing values, checked for outliers/errors, and confirmed no duplicates or mixed data types.

• **Wrangling data:**  restructured tables to have a consistent format and allow for more flexible analysis, including splitting a combined gender-ethnicity flag into two separate flags and transforming compact tables into long tables where each record/row consisted of a single data point and its related flags.

• **Merging data:**  prepared data for merge (including creating keys), confirmed merge was successful afterwards, cleaned up merged data (renaming columns, dropping flags that were no longer needed, and replacing NaNs with corrected data), and exported final merge as a pickle file.

• **Deriving new variables:** grouped data nationally by donor_type to allow comparison of sub-groups (states, genders, age-groups, ethnicities) against national norms. 

• **Exploratory data analysis:** used Matplotlib and Seaborn to explore basic statistics and potential correlations between variables via correlation heat maps, scatterplots, pair plots, and categorical plots.

• **Statistical analysis:** used the machine learning features of Scikit-Learn to apply linear regression and K-means clustering algorithms to the data to investigate a possible relationship between the rates of donations for living and deceased donors.

• **Visualizing data:** used Tableau to create a dashboard that would allow others to explore this data via interactive choropleth maps, double-bar charts, pie charts, tables, and line charts over time: https://public.tableau.com/app/profile/cj.gilbert/viz/ExploringOrganEyeandTissueDonationsintheU_S_/DonationsAcrosstheUS

• **Documenting processes:** provided an Excel file that documented the data population flow, all pre-processing steps (consistency checks, data wrangling, and column derivations), before-and-after-merging data dictionaries, and a copy of the final, fully-merged data set. 
