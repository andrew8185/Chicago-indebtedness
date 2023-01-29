
# Extraction of Chicago Employee Salaries and Indebtedness

Use Python to extract, transform, and load data into a relational database


## Authors

-[@gnimeth](https://github.com/gnimeth)
-[@bexlev](https://github.com/bexlev)
-[@andrew8185](https://github.com/andrew8185)
-[@DFandreou](https://github.com/DFandreou)
-[@bakarisimmons](https://github.com/bakarisimmons)


## Project Proposal

- The purpose of generating this combined dataset:
    - Possible analyses to be made can have relevance to the city of Chicago and their budgeting as well as how employee indebtedness is handled
    - By combining datasets, it is possible to evaluate correlations between total annual salary of a given department in the City of Chicago and the total amount of indebtedness that city employees possess, as well that between other contained variables. 
    -  The data is a relational set which can be loaded into SQL to allow for further exploration
    
## Project Report

- The data was extracted and transformed as follows:

- Datasets were downloaded as CSVs from the Chicago Data Portal and transformed to Pandas Dataframes for manipulations.

![App Screenshot](https://raw.githubusercontent.com/gnimeth/project2/main/Output/Screenshot_20230129_051806.png)

![App Screenshot](https://raw.githubusercontent.com/gnimeth/project2/main/Output/Screenshot_20230129_051903.png)

- Data from indebtedness_df was filtered to the most recent week of 1/21/23

- Department names were explored from each dataframe and manipulated to ensure seamless merge
- Hourly wages from salary_df were configured to replace all NaN under Annual Salary column.

![App Screenshot](https://raw.githubusercontent.com/gnimeth/project2/main/Output/Screenshot_20230129_051927.png)

- Annual Salaries aggregated by department and made into new dataframe, department_pay_df

![App Screenshot](https://raw.githubusercontent.com/gnimeth/project2/main/Output/Screenshot_20230129_052020.png)

- Merged department_pay_df and indebtedness_df on a right merge.

![App Screenshot](https://raw.githubusercontent.com/gnimeth/project2/main/Output/Screenshot_20230129_052035.png)

- Saved newly created dataframe to CSV
    
## Findings
- The Chicago Transit Authority has the highest number of employees indebted to the department, at 22.8 percent.
- Something alarming is how much debt the Chicago Board Of Education faces with its employees although it is a small percentage, it is a very large total figure.

## Sources

- Current Employee Names, Salaries, and Position Titles | City of Chicago | Data Portal. (2023/1/21). Data.cityofchicago.org. Retrieved January 27, 2023, from https://data.cityofchicago.org/Administration-Finance/Current-Employee-Names-Salaries-and-Position-Title/xzkq-xp2w


- Employee Indebtedness to the City of Chicago | City of Chicago | Data Portal. (2023/1/21). Data.cityofchicago.org. Retrieved January 27, 2023, from https://data.cityofchicago.org/Administration-Finance/Employee-Indebtedness-to-the-City-of-Chicago/pasx-mnuv


