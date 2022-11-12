# <b> Refactoring Stock Analysis Code </b>

## <u>Overview of Project</u>
This is an analysis of refactoring the VBA code of a stock performance analysis over past years. The original code runs in about a second but does not analyze a large number of stocks. With quicker runtime, this code could be used to analyze more and be used on a larger scale.   

### Purpose
Does refactoring the code make it run more quickly? The original code ran at 1.382813 seconds and 1.03125 seconds to analyze the 3013 rows of stock information for 12 stocks in 2017 and 2018 respectiviely. Those times are acceptable for a smaller analysis, but if the analysis needs to be expanded to the 7,290 stocks listed on the New York Stock Exchange (https://www.nyse.com/listings_directory/stock) or more, a quicker process is needed.   

## <u>Analysis and Challenges</u>
TEELL ABOUT THE DATA

### 2017 Run Time
The data showed the launch date for each campaign. During analysis, these were separated into the individual months of campaign launch. One of the research questions is whether the month of launch makes a significant difference in the outcome of the project. The graph below shows the number of successful, failed, and canceled theater projects based on the month they were launched.  

<img width="300" alt="Original_2017" src="https://user-images.githubusercontent.com/116980760/201486778-78b8ad84-dcc2-496e-86d3-af24bb441949.PNG">

<img width="300" alt="VBA_Challenge_2017" src="https://user-images.githubusercontent.com/116980760/201486787-bb29fb09-030f-4b7e-8a8a-be00025da0f5.PNG">


### 2018 Run Time
The data showed the funding goals for each campaign. One of the research questions is how the Kickstarter goals impact success. The graph below shows the percentage of successful, failed, and canceled theater projects based on the funding goal.

<img width="300" alt="Original_2018" src="https://user-images.githubusercontent.com/116980760/201486856-f8c5ee01-0dad-4813-944d-d2658eb47b83.PNG">

<img width="300" alt="VBA_Challenge_2018" src="https://user-images.githubusercontent.com/116980760/201486816-44f706f8-5a2d-4766-9c14-2bec66dda269.PNG">

### Challenges and Difficulties Encountered

Some of the data was not in an user-friendly format. Dates originally had Unix timestamps and had to be converted to human-readable dates. Parent categories and subcategories were combined in one column and had to be separated for easier analysis. 



## <u>Results</u>

- The new code was % faster than the original.

- Refactoring the code made it much more efficient. 


