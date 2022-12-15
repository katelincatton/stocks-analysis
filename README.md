# Stock Analysis (2017 and 2018)

## Overview of Analysis

This analysis was performed and prepared to overlook the stock market for 2017 and 2018. The analysis was ran to determine the total daily volume and stock return by ticker. A stock ticker is a pricing report for certain seecurities and is made up of unique series of letters (https://www.investopedia.com/ask/answers/12/what-is-a-stock-ticker.asp); We have 12 tickers in our dataset, in otherwords, 12 different stocks. With this dataset, we hope to find stock outputs for both 2017 and 2018 for all tickers. By refactoring the previous code used, we hope to limit the excution time of the analysis so that the macro will be able to handle thousands of stocks if needed in the future.

## Results
### Analysis
By examining the previous code, the code must be refactored to make the run-time faster. This analysis will describe each step that was taken to create a faster and more efficient macro; This includes a ticker index variable, three output arrays, for loops, if-then statements, and much more. Once the code has been completed, the macro will allow us to analyze the stock outcomes.

#### 1a. Creating a tickerIndex variable and set it equal to zero
---
![image](https://user-images.githubusercontent.com/119131202/207751402-4e21ee77-8ff4-46a4-8d81-346d39b8c1e3.png)
---
#### 1b. Creating three output arrays: tickerVolumes, tickerStartingPrices, and tickerEndingPrices
---
![image](https://user-images.githubusercontent.com/119131202/207752290-29586d4c-4b12-421b-bd64-ccc09cfa6070.png)
---
#### 2a. Create a for loop to initialize the tickerVolumes to zero
---
![image](https://user-images.githubusercontent.com/119131202/207752576-e366c0d1-2afb-4118-8516-103eeb43299c.png)
---
#### 2b. Create a for loop that will loop over all the rowa in the spreadsheet
---
![image](https://user-images.githubusercontent.com/119131202/207752717-25d110e9-811f-437e-b3c0-93ae3e060e4a.png)
---
#### 3a. Inside the for loop above, increase the current tickerVolumes variable and add the ticker volume for the current stock ticker
---
![image](https://user-images.githubusercontent.com/119131202/207752976-167de7af-9279-4151-8a01-7465de86b228.png)
---
#### 3b. If-then statement to check if the current row is the first row with the selected tickerIndex. If it is, then assign the current starting price to the tickerStartingPrices
---
![image](https://user-images.githubusercontent.com/119131202/207753248-21031446-0f4f-43ed-a31f-b8d02158d918.png)
---
#### 3c. If-then statement to check if the current row is the last row with the selected tickerIndex. If it is, then assign the curent closing price to the tickerEndingPrices variable.
---
![image](https://user-images.githubusercontent.com/119131202/207753483-01dcdc2b-9690-435b-a02f-4e26237e4049.png)
---
#### 3d. Write a script that increases the tickerIndex if the next rows ticker doesn't match the previous rows ticker
---
![image](https://user-images.githubusercontent.com/119131202/207753724-2adfd566-3155-465d-a247-1e2c009f89b1.png)
---
#### 4. Use a for loop to loop through your arrays to output your three arrays
---
![image](https://user-images.githubusercontent.com/119131202/207753774-28eefbde-2c06-4245-bac7-9e7efbefe339.png)
---
---
With a succesful macro, it has allowed us to examine the daily volume and returns for all stocks in 2017 and 2018. The stocks from 2017 tend to have a higher return when compared to the 2018 stocks. Even the stocks with lower daily volumes had a high return rate. Nearly all stocks in 2017 had a positive return, except the stock ticker "TERP". The 2017 stocks had many stocks that had a return greater that 100%, which allows us to say that the 2017 stocks (except TERP) are good and reccomended. 
---
#### 2017
![Stock_Output_2017](https://user-images.githubusercontent.com/119131202/207757849-075fc2c1-d5e0-4f02-ae3c-4af6463742e1.PNG)
---
The stocks in 2018 were nearly all negative except two stocks: "ENPH" and "RUN". These two stocks had a fairly high return, but it's not much when compared to 2017 returns. These two stocks had a large daily volume, which ultimately helped with their return rate. With negative returns, you may want to shy away from buying these stocks in 2018.
---
#### 2018
![Stock_Output_2018](https://user-images.githubusercontent.com/119131202/207757878-5feabf4b-fc2c-4870-89bf-7fd4178700a8.PNG)
---
## Summary
### 1. What are the advantages or disadvantages of refactoring code?
---
There are many reasons as to why a programmer would want to refactor the original code. One of the biggest reasons being the decreased exucution time. When refactoring code, it often breaks down the code into smaller and more workable code. In result, this leads to faster run-time with the same accurate outputs. For example, after refactoring this code, the run-time has been 0.168 seconds for the 2017 stocks and 0.156 seconds for 2018 stocks; Both of which are much lower than the previous run-times, where the previous run-times were almost one second.
---
#### 2017
![VBA_Challenge_2017](https://user-images.githubusercontent.com/119131202/207760130-02f6838c-5d92-47e1-87f2-c22d03d81ec7.PNG)
---
##### 2018
![VBA_Challenge_2018](https://user-images.githubusercontent.com/119131202/207760163-6faacbb2-563a-4489-9711-c9204fe13dd5.PNG)

### 2. How do these pros and cons apply to refactoring the orignal VBA script?
The act of refactoring allows for both the programmer and the people viewing the code, to more easily read and intepret the code. It makes it easier to understand what is happening in each step as the code runs through. It also allows the system to execute at a faster rate due to less formulas and lines to run through. The refactored code ultimately creates a cleaner way of programming and allows for an easier way of debugging along the way. Well it's obvious that refactoring code can be very beneficial, it's not always an option. Some programmers may run into issues where their dataset is too large and it's too difficult to test the code before making changes. Additionally, some code may have no option but to be long and difficult, due to having lots of steps to complete what is neccesary. In conclusion, always revert to refactoring your code if possible!
---
---
Analysis Performed by Katelin Catton
---
12/15/2022
