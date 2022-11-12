# <b> Refactoring Stock Analysis Code </b>

## <u>Overview of Project</u>
This is an analysis of refactoring the VBA code of a stock performance analysis over past years. The original code runs in about a second but does not analyze a large number of stocks nor much accompanying information. With quicker runtime, this code could be used to analyze more and be used on a larger scale.   

### Purpose
Does refactoring the code make it run more quickly? The original code ran at 1.382813 seconds and 1.03125 seconds to analyze the 3013 rows of stock information for 12 stocks in 2017 and 2018 respectiviely. Those times are acceptable for a smaller analysis, but if the analysis needs to be expanded to the 7,290 stocks listed on the New York Stock Exchange (https://www.nyse.com/listings_directory/stock) or more, a quicker process is needed.   

## <u>Analysis and Challenges</u>
The initial code has nested for loops. In the new code, it loops over the data only once which significantly improved run time. The original code initializes a ticker value. Then checks to see if each row has the same ticker and if so, adds it to the total volume. It also checks to see if it is the first or last row with the specific ticker. After it checks through all of the rows of data, it displays the values, the ticker value is updated, and variables are reset. The process repeats for each of the 12 different stocks. The new code has an array to store the different values for each different ticker. Instead of resetting the variable and looping through for each ticker, it gets the values on the initial loop for all of the stocks at once.

### 2017 Run Time
The images below show the run time on the original and the new. The run time on the original 2017 stock data analysis was 1.382813 seconds and the new run time is 0.1367188 seconds, which means it improved the running time by one magnitude. 

<img width="300" alt="Original_2017" src="https://user-images.githubusercontent.com/116980760/201486778-78b8ad84-dcc2-496e-86d3-af24bb441949.PNG">

<img width="300" alt="VBA_Challenge_2017" src="https://user-images.githubusercontent.com/116980760/201486787-bb29fb09-030f-4b7e-8a8a-be00025da0f5.PNG">


### 2018 Run Time
The images below show the run time on the original and the new. The run time on the original 2018 stock data analysis was 1.03125 seconds. The new run time is 0.1367188 seconds. The running time was about 8 times as fast. 

<img width="300" alt="Original_2018" src="https://user-images.githubusercontent.com/116980760/201486856-f8c5ee01-0dad-4813-944d-d2658eb47b83.PNG">

<img width="300" alt="VBA_Challenge_2018" src="https://user-images.githubusercontent.com/116980760/201486816-44f706f8-5a2d-4766-9c14-2bec66dda269.PNG">

### Challenges and Difficulties Encountered 
The original code performed as it should. The challenge was finding a way to make the process more efficient. Looping through the information for each stock gave the needed information, but there was a better way.

## <u>Results</u>

- The new code was about 8 to 10 times faster than the original.

- Refactoring the code made it much more efficient. 


