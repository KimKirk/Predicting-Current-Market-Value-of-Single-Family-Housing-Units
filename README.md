# HADS_Predicting-Current-Market-Value-of-Single-Family-Housing-Units
- Predicting current market value of single family housing units
- Finance: Housing

- All files are self-contained analysis reports that include necessary variables.

- Many businesses still use Excel as a primary "database"/data storage device; to accomodate this, all files are Excel based and analysis was run using Excel.

- Inferential data analysis was conducted using multivariate linear regression to predict current market value of single family housing units for 2013. 


## Processing Instructions:
- Use Excel or application that can open .xlsx files to view the analysis report.
- Each worksheet is labeled to include "Summary Report", "Descriptive Statistics", "Graphs/Charts", and "Statistical Test".
- Data Analysis Report is in pdf.
- Codebook is in pdf.


## Steps to Transformation:
### Data was tidied by:
- Dataset was downloaded from host website: https://www.huduser.gov/portal/datasets/hads/hads.html
- Data was cleaned to include only single-family houses, flats, apartments with Fair Market Value of more than $1000.00 owned in 2013 as this was the subset that stakeholders wanted to focus on.
  - Missing values made up 4.1% of the data and were discarded per stakeholder input.
- VALUE 2013 was determined to be the outcome variable.
- AGE 2011, METRO3, REGION, LMED_2011, FMR_2011, VALUE_2013, BEDRMS 2011, BUILT_2011, VALUE_2011, ROOMS 2011, PER 2011, ZINC2_2011, ZADEQ_ADEQUACY, UTILITY_2011, OTHERCOST_2011 were determined to be the predictor variables.
- LMED_2011, OTHERCOST_2011, FRM_2011, BUILT_2011, VALUE_2013, PER_2011, ZINC2_2011, UTILITY_2011 had exponential distributions and a natural logarithmic transformation was applied for a normal distribution.
- New variables created include:
  - LN_LMED_2011
  - LN_FMR_2011
  - LN_VALUE 2013
  - LN_BUILT_2011
  - LN_VALUE_2011
  - LN_PER 2011
  - LN_ZINC2_2011
  - LN_UTILITY_2011
  - LN_OTHERCOST_2011
- 1000 observations were randomly selected as Test data; the rest of the data set was used as Training data for the predictive model.
- Worksheets were created to hold four categories for the analysis:
  - Summary Report identifies and answers the business question/what was measured
  - Descriptive Statistics identifies and calculates descriptive statistics
  - Graphs & Charts displays histograms, scatterplots, bar graphs
  - Statistical Tests holds results for statistical tests
