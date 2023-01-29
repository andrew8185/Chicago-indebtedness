# Project 2: Extract, Transform, and Load

## Authors

-[@gnimeth](https://github.com/gnimeth)
-[@bexlev](https://github.com/bexlev)
-[@andrew8185](https://github.com/andrew8185)
-[@DFandreou](https://github.com/DFandreou)
-[@bakarisimmons](https://github.com/bakarisimmons)


# PROJECT PROPOSAL

The purpose of generating this combined dataset:

    By combining datasets, it is possible to evaluate correlations between total annual salary of a given department in the City of Chicago and the total amount of indebtedness that city employees possess, as well that between other contained variables. 
    
    The final production database to load the data into is prepared to load into SQL, so is relational.

Findings:	

    -When it comes to the highest percentage of employees in debt it is the Chicago Transit Authority At 22.8 percent of their employees are in debt.
    -Something that was alarming is how much debt the Chicago Board Of Education faces with its employees although it is a small percentage, it is a very large total figure.
    -Although it would be very interesting to see how much one employee is in debt to their public sector it is intriguing to see the percentage of debt to Chicago.

Citations:
    
    -Current Employee Names, Salaries, and Position Titles | City of Chicago | Data Portal. (n.d.). Data.cityofchicago.org. https://data.cityofchicago.org/Administration-Finance/Current-Employee-Names-Salaries-and-Position-Title/xzkq-xp2w

    -Employee Indebtedness to the City of Chicago | City of Chicago | Data Portal. (n.d.). Data.cityofchicago.org. Retrieved January 27, 2023, from https://data.cityofchicago.org/Administration-Finance/Employee-Indebtedness-to-the-City-of-Chicago/pasx-mnuv



# PROJECT REPORT
The data was extracted and transformed as follows:
      -Datasets cited above were downloaded as CSVs from the Chicago Data Portal as uploaded as Pandas Dataframes for manipulations.
      -In order to merge the dataframes in order to compare, manipulations were required.This included changing Department names to be the same between data sets in order to facilitate merging without losing any information for departments.
      -To expand the dataset's usefulness post-merged, we found the yearly sum of salaries of each department and compared to total indebtedness.


This topic was chosen at a professional level because the analyses that could be made could have relevance to the city and their budgeting as well as how employee indebtedness is handled.

