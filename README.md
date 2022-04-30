# Analyzing 10Gb of Yelp Reviews Data

For this project, I used a Spark Cluster on AWS EMR for loading and running some analysis on Yelp’s Reviews and Businesses dataset (about 10gb) from Kaggle. I run my analysis via Jupyter Notebook and the expected output artifact is Analysis.ipynb file.

**Technology used**
Python (Spark SQL)


**Cluster Configuration**
![Alt text](https://github.com/jinote/yelp-analysis-project/blob/main/cis9760-yelpcluster.jpg)

**Notebook Configuration**
![Alt text](https://github.com/jinote/yelp-analysis-project/blob/main/cis9760-yelpnotebook.jpg)

**Part I: Installation and Initial Setup**<br>
In this portion, I imported the necessary dependencies (pandas and matplotlib, seaborn is optional) and loaded the dataset as a pyspark dataframe.

**Part II:  Analyzing Categories**<br>
For this part, I took a stab at denormalizing the categories that are associated with each business (there may be more than one, presented as a string of comma separated identifiers) and then running some basic analysis on the result.

**Part III: Do Yelp Reviews Skew Negative?**<br>
For this next part, I attempted to answer the question: are the (written) reviews generally more pessimistic or more optimistic as compared to the overall business rating. There are some required questions you must answer (see the analysis.ipynb file) which is the bare minimum. 

**Part IV: Should the Elite be Trusted?**<br> 
For this final part I explored the data and calculated the difference bewteen business actual ratings and elite users' ratings. 
-	I leveraged the users dataset provided
-	I crated one visualization 
