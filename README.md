# nonsql_challenge


#part 1

I imported the dependencies and created an instance of MongoClient. I assigned the uk_food database and the establishments collection a variable.

#part 2

Here I added the new restaurant "Penang Flavours" to the collection and updated its BusinessTypeID to 1.

I also deleted any establishments in Dover and updated 'latitude' and 'longitude' to floats. 

#part 3

In part 3 I queried which establishments have a hygiene score equal to 20 and used count_documents() to list the number of documents. Then the results were converted into a Pandas DataFrame. 

Then,I queried which establishments in London have a RatingValue greater than or equal to 4. I used the $regex operator to locate the London establishments, count_documents() to list the number of documents, and then coverted the results into a DataFrame.

Next, I queried for the top 5 establishments with a RatingValue of 5 and sorted the resultsin ascending order based on the hygiene score. I limited to results to 5, and then I converted the results into a DataFrame.

Lastly, I queried for how many establishments in each Local Authority area have a hygiene score of 0 by creating an aggregation pipeline to get the documents that matched the query, then grouped by LocalAuthorityName, and lastly sorted the count of the documents in descending order. I used the aggregate method for the aggregation pipeline, casted the results to a list, and printed the first 10 results.  In the end, I converted the results into a Pandas DataFrame.
