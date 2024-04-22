# data-sourcing-challenge
Week 6 Challenge

# Functionality:
This application queries the New York Times API movie reviews based on filter criteria and returns 200 JSON results into a list. Those results are lightly transformed to isolate the title and extract keywords. Those results are then placed into a dataframe and the titles are used to feed a query into two The Movie Database APIs. The application first loops through the titles and requests the movie id. Once the id is determined, it further requests details via a second API endpoint to obtain various information such as genres, spoken languages, and production countries for each title. These JSON results are then converted to a dataframe. The applications then merges the two dataframes into one dataframe and performs data clean up. Once complete, the application produces the final output, which is a csv file. 

![Screenshot](top_5_client_summary.png)

# Approach:
The approach consisted of three steps.
1. Query and obtain the NYT reviews list using the filter criteria and their API. Store these results in a dataframe and create a list to pass in step 2.
2. Make the first of two TMDB calls looping through the titles list from the NYT in order to get the id, one movie at a time. Then, within the same loop, make a second call with a different NYT API to obtain details for each movie id. Store these results in a list and convert to a dataframe.
3. Merge the two dataframes into one and perform clean up tasks. Once clean, export the merged dataframe to a csv file.

# Summary of Findings:
The data showed that the top five most active clients purchased 496,628 items, generated $123,556,060 in revenue, and contributed $48,045,451 to profit. A single client generated 48.3%, 66.6%, and 76.1% of those amounts respectively. There is significant concentration risk in the one single client. It is recommended to reduce the concentration risk of this single client.

# Plagerism Statement:
No specific code was copied but the sources below were referenced for examples and syntax. 

# Sources:

Applying lambda row on multiple columns pandas. (n.d.). Stack Overflow. Retrieved April 4, 2024, from https://stackoverflow.com/questions/51080174/applying-lambda-row-on-multiple-columns-pandas

Harrison, M. (2021). Effective Pandas: Patterns for Data Manipulation. Matt Harrison.

Lutz, M. (2013). Learning python: Powerful object-oriented programming. " O'Reilly Media, Inc.".


