Nexus of Crisis: Examining the opioid epidemic and various demographic factors
---
This README contains both:

**1. Analysis and Conclusion**

**2. Installation Instructions**
   
---
**1. Analysis and Conclusion**

The number of opioid-related deaths has been rising continuously since 1999. The number of people who died from a drug overdose in 2021 was over six times the number in 1999. Over 75% of the nearly 107,000 drug overdose deaths in 2022 involved an opioid.

Against this background, this project examines the opioid epidemic and explores if there is any correlation between opioid-related deaths and various demographic factors, namely unemployment rate, educational attainment, income level and family size.

1.1 Analysis

1.1.1. _What is the trend in opioid deaths across the USA?_

**Our findings**: Opioid death counts have been rising year over year. California and Florida have seen the sharpest rise in opioid death counts (CDC 2017-2022)

1.1.2 _Can unemployment levels in a given state possibly correlate to opioid deaths counts in that state? Could unemployment predict levels of opioid death?_

**Our findings**: To conduct this analysis we used US Census data extracting 5 years of total unemployed in the civilian labor force to identify percent contributions by state population. We then calculated the percent conribution of opioid related death counts per state to population numbers and then analyzed the ratio in a heatmap to see if there is any potential correlation between the rates. We did not conclude that there is necessarily a strong relationship but we did identify the states that have much higher death rates to unemployment that would be worth investigating further to understand what IS causing such high numbers. The pie charts reflect the percent to total 5 years by year contribution to unemployment in the total US and opioid related death counts by year in total US. We singled out year 2022 as the unemployment rates were the highest of all 5 years as the opioid related deaths were second lowest as well as half of the unemployment rate in that year. Based on the findings or lack there of, we cannot suggest that unemployment has a relationship to opioid related deaths, if we were to conduct this analysis further we would identify the unemployment status of the specific persons that are counted for opioid related deaths and then be able to make a more accurate assumption.

1.1.3 _Can educational attainment in a given state possibly correlate to opioid deaths counts in that state? Could educational attainment be a predicter for levels of opioid death?_

**Our findings**: To conduct this analysis we analyzed educational attainment data from the US Census. Educational Attainment was grouped into those who never graduated high school, those with high school/GED, those with a college degree, and those with an advanced degree.

We conducted a regression analysis to determine if there was a possible correlation between educational attainment and opioid death. Two single variable regressions (opioid deaths and % of state with college degree, opioid deaths and % of state with high school diploma/GED) revealed there is no correlation between these two variables. The regression line was flat.

1.1.4 _Can median household income in a given state possibly correlate to opioid deaths counts in that state? Could median household income be a predicter for levels of opioid death?_

**Our findings**: To conduct this analysis we analyzed median household income data from the US Census.

We conducted a regression analysis to determine if there was a possible correlation between median household income and opioid deaths. Two single variable regressions (opioid deaths and median household income) for five years (2017-2019, 2021-2022) and for each year revealed there is weak to no correlation between these two variables. The regression lines were slightly positive or flat. 

To validate the weak correlation, we further conducted t test and ANOVA for opioid death in above-average income group (states with median household income above the national average) and below-average income group (states with median household income below the national average). As there is no statistically significant difference, we concluded that income level does not have a statistically effect on opioid deaths.


1.1.4 _Can average family size in a given state possibly correlate to opioid deaths counts in that state? Could family size be a predicter for levels of opioid death?_

**Our findings**: To conduct this analysis we compared various households which we acquired data from the US Census to opioid deaths across the United States. These households were narrowed down to focus on households living alone.

We prepared a series of scatterplots to ascertain if there is a correlation between households living alone and opioid deaths. 2017-2019 and 2021-2022 all showed a distinct correlation individually and collectively between living alone and opioid deaths. The regression line for every year was pointing in a positive direction. Family size could be a good predicator of future opioid deaths.


1.2 Conclusion

Lack of correlation highlights the complexity of the opioid epidemic, necessitating a multifaceted approach to prevention and treatment. Additional analysis could be conducted to determine if a combination of these factors is a better predictor of overdose outcomes in a state. More analysis should be completed to examine other demographic factors or alternative data, such as prior hospitalizations/surgeries and overdoses.

**2. Installation Instructions**

2.1. Dependencies

2.1.1. Software needed Please have the following software installed on your system:

Operating systems: Windows, macOS, or Linux
Programming languages: Python (version 3.7 or higher recommended)
Development tool: Jupyter Lab (for interactive development and notebook execution)
Other tools: Git (for version control)
2.1.2. Libraries needed Please have the following Python libraries installed using pip:

pandas: for data manipulation and analysis
geopandas: for working with geospatial data
matplotlib: for creating visualizations and plots
numpy: for numerical operations and array handling
requests: for making HTTP requests
scipy: for statistical functions and linear regression
2.2. Setup Steps

First, clone the repository to your local machine using Git: git clone https://github.com/kikichan1/Project-1.git
Navigate into the project directory: cd Project-1
Create a virtual environment: python -m venv venv (on Windows) venv\Scripts\activate (on macOS/Linux) source venv/bin/activate
Install dependencies pip install -r requirements.txt
Install Jupyter Lab pip install jupyterlab
2.3. Usage Instructions

Activate the developer environment and open start Jupyter Lab conda activate dev jupyter kernelspec list jupyter lab
Input your API key in api-keys.py
Restart the kernel
Run the code
2.4. Features The project has the following main features:

Data manipulation and analysis: utilize the pandas library to perform data manipulation and analysis tasks, including data import, cleaning and analysis
Data visualization: use matplotlib to generate plots and charts, such as line graphs and scatter plots
Numerical operations: Perform numerical computations and statistical functions using numpy and scipy respectively
HTTP requests: make HTTP requests and interact with web APIs using the requests library, and fetch and integrate data from external sources into the analysis
2.5. Contributing

2.5.1. Bug reports and feature requests If you find a bug or have a feature request, please contact the authors via email.

2.5.2. Questions and feedback If you have any questions or feedback, please contact the authors via email.

2.6. License This project is licensed under the MIT License. You can freely use, modify, and distribute the code as long as you include the original copyright and license notice in any copies or substantial portions of the software. For more details, please see the LICENSE.md file.

2.7. Contact Information Rachel Brown (email: r.erin.brown@gmail.com) Elizabeth Conn (email: elizabethlconn@gmail.com) Kiki Chan (email: kiki.puikichan@gmail.com) Sara Roulett (email: sroulett@gmail.com)

2.8. Acknowledgements We would like to express our thanks to our course instructors Gurpreet Sodhi and Bomin Kwon for their valuable feedback.
