
# Applied Data Analytics

## Wedge Project

<!-- Any general commentary you'd like to say about the project --> 

I am currently turning in Task 1 and Tast 2 to you for review. I have filled in the Query Comparison Results below, and have some 
slight differences on a couple of the queries. Still working on Task 3 but will update this file and ReadMe when I get that done. 

### Task 1

* Files for this task: 
<!--  List of file or files here  --> 

Clean ZipFiles containg Wedge data

`File1 Name`: Wedge Cleaning Final.ipynb

Opened the Zip files containing the Wedge data for each month from 2010 to 2017. Cleaned the files by eliminating certain delimiters, 
removing unwanted null values like "\\n" and adding headers to each new cleaned cloumn. Then writing the cleaned data to a new folder 
named 'wedge_clean'.

<!--  Repeat for each file  --> 

Loads all data into GBQ data set.

`File2 Name`: Wedge GBQ Import Code.ipynb

Upload the new cleaned files to GBQ. This involed connecting to GBQ to access my project 'wedge2020' and dataset 'wedge_transactions_data'. 
Then using a schema to create tables in that dataset, I was able to configure a GQB job to upload my local cleaned files into those tables. 

### Task 2

* Files for this task: 
<!--  List of file or files here  --> 

Taking a sample of owners from GBQ

`File3 Name`: Task 2 - A Sample of Owners.ipynb

I again connected to my project in GBQ and ran a query to pull all the owners using "card_no" and remove the non-owners who were recorded 
under card_no 3. I then used the random() function to pull a sample of owners from the total card_no and wrote this sample to 
'owner_transactions.txt' which I will use to complete task 3. 

<!--  Repeat for each file  --> 
	

### Task 3

* Files for this task: 
<!--  List of file or files here  --> 

Loads all data into GBQ data set.

`File1 Name`: 
Description of what this file does.

<!--  Repeat for each file  --> 


## Query Comparison Results

Fill in the following table with the results from the 
queries contained in `gbq_assessment_query.sql`. You only
need to fill in relative difference on the rows where it applies. 
When calculating relative difference, use the formula 
` (your_results - my_results)/my_results)`. 



|  Query  |  Your Results  |  My Results | Difference | Rel. Diff | 
|---|---|---|---|---|
| Total Rows  | 85760124 | 85760139 |  15 |  1.749064329291724e-7 |
| January 2012 Rows  | 1070907  |  1070907 | 0 | 0  |
| October 2012 Rows  |  1042287 |  1042287 | 0  | 0  |
| Month with Fewest  | February  |  February | No  | NA  |
| Num Rows in Month with Fewest  | 6556769  |  6556770 |  1 |  1.525141189945659e-7 |
| Month with Most  |  March | March  | No  | NA  |
| Num Rows in Month with Most  |  7578371 | 7578372 | 1  |  1.319544619873503e-7 |
| Null_TS  | 7123787  | 7123792  | 11  | 1.544121445432433e-6 |
| Null_DT  |  0 |  0 | 0  |  0 |
| Null_Local  | 234843  |  234843 | 0 |  0 |
| Null_CN  |  0 |  0 | 0  | 0  |
| Num 5 on High Volume Cards  | 14987.0  | 14987.0  | No  | NA  |
| Num Rows for Number 5 |  460630 |  460630 |  0 | 0 |
| Num Rows for 18736  | 12153  | 12153  |  0 |  0 |
| Product with Most Rows  | banana organic  | banana organic  | No | NA  |
| Num Rows for that Product  | 908637  | 908639  |  2 |  2.201094163908879e-6 |
| Product with Fourth-Most Rows  | avocado hass organic  | avocado hass organic  | No  | NA  |
| Num Rows for that Product  | 456771  | 456771  |  0 |  0  |
| Num Single Record Products  |  2769 | 2769  |  0 |  0  |
| Year with Highest Portion of Owner Rows  |  2010 |  2010 | No | NA |
| Fraction of Rows from Owners in that Year  | 0.7422  | 0.7422  |  0 | 0  |
| Year with Lowest Portion of Owner Rows  |  2017 |  2017 | No | NA |
| Fraction of Rows from Owners in that Year  |  0.7513 |  0.7513 | 0  |  0 |

## Reflections


<!-- I'd love to get 100-200 words on your experience doing the Wedge Project --> 
