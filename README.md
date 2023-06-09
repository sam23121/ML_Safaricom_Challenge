### Ml safaricom Challenge

The Notebook "ml_safaricom.ipynb" describes each step for the challenge

- The first answer Reads the Csv "OnlineRetail.csv" into a dataframe then sortes the dataframe by the date column and displays the top 7 and the last 12 rows of the dataframe using DataFrame.head()
- The second I dropped the rows the null values in the CustomerId column
- The third is adding a new feature by multpliying the Quatity and UnitPrice column and assing it to a column called SaleValue
- The forth is calulating the Recency, Frequency and Monetary value per CustomerId (by DataFrame.grouping())
- The fifth using a clustering model of choice which I choose k-means and before determining the number of centroids I used wcss (within clustering sum of squares). after the number of centroids is determined I used "k-means++" to initlliaze the postions of the centroids
- The sixth I aggregate the three values by adding the recency, frequency and monetary and divde them by three (taking the average of the 3 columns) and assinging it a new column called OverallScore
- the seventh I plotted 3 plots which is recency vs overall score, frequency vs overallscore, monetary vs overallscore
- the eigth I wrote a function that assigns labels based on the OverallScore column using DataFrame.apply() (for vectorization) and assign it to a column called Segment, and at last save the Dataframe to a csv file called "Customer_Segmentation_Analysis.csv"