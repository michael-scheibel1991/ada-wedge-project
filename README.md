# ada-wedge-project

**Task 1: Building a Reporting Database in Google Big Query**

First part of task one was opening the Zip files containing the Wedge data for each month from 2010 to 2017. 'Wedge Cleaning Final.ipynb' shows the code for taking these files and cleaning them up by eliminating certain delimiters, removing unwanted null values like "\\n" and adding headers to each new cleaned cloumn. Then writing the cleaned data to a new folder named 'wedge_clean'.

Second part of task one was to upload these new cleaned files to GBQ using 'Wedge GBQ Import Code.ipynb'. This involed connecting to GBQ to access my project 'wedge2020' and dataset 'wedge_transactions_data'. Then using a schema to create tables in that dataset, I was able to configure a GQB job to upload my local cleaned files into those tables. 


**Task 2: A Sample of Owners**

My code for this task is in 'Task 2 - A Sample of Owners.ipynb' and the file that contains the sample of owners is 'owner_transactions.txt'.
I again connected to my project in GBQ and ran a query to pull all the owners using "card_no" and remove the non-owners who were recorded under card_no 3. I then used the random() function to pull a sample of owners from the total card_no and wrote this sample to 'owner_transactions.txt'.


**Task 3: Building Summary Tables**

For this task I put together three queries that were ran against my uploaded wedge data, and generated three tables:  Sales by date by hour, Sales by owner by year by month and Sales by product description by year by month. I then exported these table to text files locally. I then wrote Python script that created three blank tables in a new database: "wedge_task3.db" and then filled those table with the data from teh three text files I exported. 




