# Star Wars Script
---

***Project Proposal***

  In this assignment, we were tasked with combining two or more data sources and migrating themm into a database, preferably a doucment-orientd database program: MondgoDB.

***Data Cleanup and Analysis***

+ EXTRACT (Sources)

https://www.kaggle.com/xvivancos/star-wars-movie-scripts

 From this source we retrieved .txt files of the scripts from the first three Stars Wars films (i.e. Episode IV, Episode V, and Episode VI).

http://www.omdbapi.com/

  From this source we retrieved JSON-formatted data of the first three Star Wars films.
  
+ TRANSFORM

 Kaggle Data:
  We first converted the txt files into Panda dataframes, then manipulated the data by adding columns (the specific movie title). We finally concatenated the three seperate movie dataframes into one dataframe (to allow for easier processing) and made that DF into a dictionary to allow for updating into MongoDB.
  
OMDB Data:
  We retrieved the movies ids from the OMDB API site, then made a loop that puts the data into a list of dictionaries for processing with MongoDB.
  
+ LOAD

![OMDB screenshot](Images/OMDB_mongo.png)
 
 
