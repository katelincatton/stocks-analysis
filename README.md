# Stock Analysis (2017 and 2018)

## Overview of Analysis

This analysis was performed and prepared to overlook the stock market for 2017 and 2018. The analysis was ran to determine the total daily volume and stock return by ticker. A stock ticker is a pricing report for certain seecurities and is made up of unique series of letters [GitHub Pages(https://www.investopedia.com/ask/answers/12/what-is-a-stock-ticker.asp); We have 12 tickers in our dataset, in otherwords, 12 different stocks. With this dataset, we hope to find stock outputs for both 2017 and 2018 for all tickers. By refactoring the previous code used, we hope to limit the excution time of the analysis so that the macro will be able to handle thousands of stocks if needed in the future.

## Results
### Analysis
By examining the previous code, the code must be refactored to make the run-time faster. This analysis will describe each step that was taken to create a faster and more efficient macro; This includes a ticker index variable, three output arrays, for loops, if then statements, and much more.

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
##Summary


Analysis Performed by Katelin Catton
12/15/2022
