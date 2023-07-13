# Efficient Yelp API Calls 
 
For this project we worked with the Yelp API to search for our favorite city for a cuisine type. The city used was Denver and the cuisine type was pizza. 

We extracted all of the results from the search and compiled them into one dataframe using a for loop. 

During the work we ran into an issue 'YelpAPIError: VALIDATION_ERROR: Too many results requested, limit+offset must be <= 1000.'

To solve this and handle the queries with >1000 results we deleted previous results by using 'os.remove' and stopping the loop whenever it exceeded 1000 API calls. Once this was done duplicates were purged out and the final dataframe was saved in the data folder. 