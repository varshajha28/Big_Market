# Big_Market
Extarct : The data for this challenge was available in the S3 bucket of the AWS environment : The dataset has the reviews about Musical Instrument being sold on the amanzon website. The count showed that there are 904765 rows in the dataset.

Transform: For this challenge I chose the dataset with reviews about Musical Instrumentbeing sold on the amazon website . The first step in the data cleaning process was to drop the null values in the dataset.This reduced the count to 904663. Then I removed the duplicates from the whole data set. Next part of the transform process was to create the dataframes for each of the Postgres SQL tables in AWS environment. This step also included me to check the data type of each of the columns matches the columns available in the postgres tables. I modified the "review data" format for the whole dataframe . The next step was to ensure that all the primary key columns had unique values and the customer table had total customer count.

Load : Once the data was cleaned and modified then I load it to the various dataframes into the respective tables in the postgres data table and into the RDS environment in AWS. I also verified the result form the pgAdmin.
## Resources
- Data Source: 

- Software: AWS RDS and S3, Google collab, Hadoop, Map Reduce and Python .
 ## Link to the source code and project :
a. [ETL](https://colab.research.google.com/drive/11QTW6XWE9255XLiOrZLwX2Ra0eU8cmNU#scrollTo=2UlkbMkKXJms)
b. [Statistics](https://colab.research.google.com/drive/12pwczLyEJoWoYwEdIDabRZxzfekroBkG#scrollTo=eIpI1oatRETS)

## Final Analysis:
Objective:The Statistical Analysis of the vine review in the dataset was to analyze the data and determine if the Vine reviews are biased or not.

Population: We included the clean data without the null value and duplicates . The dataset was further sampled to include only those instrument which had total votes count more than 20. The data sample was further filtered which had at more than 50 % of helpful votes compared to the total votes .

Analysis: We divided the final sample in two categories Category 1 : The data with vine = 'Y'- These means that the votes provided was apart of reward program. Category 2 : The data with vine = 'N'- These means that the votes provided was not apart of reward program.

Conclusion: The Category 1 had a total count of 60 , the mean for star_rating was 4.38, helpful_votes 40.22 and total_votes was 45.9. The percentage of the five star rating in this category was 56.67%.

Where as, the Category 2 had a total count of 14473, the mean for star_rating was 4.05, helpful_votes 47.5 and total_votes was 51.8. The percentage of the five star rating given in this category was 56.77%.

Final conclusion: The percentage of the five star rating given by the vine review as yes and the five star rating given by the vine review as no is only 4%. The review are not biased as the large popualation were not a part of the reward program have still given five star rating and those reviews were reported helpful by a significant number of people .
