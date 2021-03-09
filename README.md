# Green stock analysis code refactor
##Explain the purpose of this analysis:
Provide analysis to Steve to help him figure out the performance of different stocks.

## Result:
###### original script VS. script after refactor
The original script read the whole data once for each different ticker. The total number of rows it will read is the total number of tickers time the total number of row information. After refactoring the code, the script will run all the information once. The total volume will be added up for each ticker and when the ticker index is changed, the volume will be added up into the new ticker index’s total volume. Therefore, the performance is more efficient than the original one.
###### 2017 VS. 2018 return
After comparing the return between 2017 and 2018, we can see only ticker “ENPH” and ticker “RUN” have the positive return for both years. It means that their performance is better than other stocks.
## Summary:
###### Advantage: 
The refactoring code will only read the code once which mean that the running time for the script is less than the original code
###### Disadvantage：
The refactoring code is based on the data is sorted before we run the program. The original code can have the correct result even though the tickers are not sorted.




