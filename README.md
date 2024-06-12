# NoSQL_Challenge
This repository contains the work covered in NoSQL database activities.

## Part 1: Database and Jupyter Notebook Set Up
Completed the following tasks for setting up the database and Jupyter notebook:

1. Included the mongoimport command text used to import establishments.json in a markdown cell at the beginning of the Jupyter notebook file.
2. Ensured that the mongoimport command text correctly dropped any existing establishments collection before importing establishments.json into MongoDB.
3. Named the database uk_food and the collection establishments.
4. Imported PyMongo and Pretty Print libraries.
5. Created an instance of the Mongo Client.
6. Listed the databases in Mongo, which included uk_food.
7. Listed the collection(s) in the uk_food database, which included establishments in the output.
8. Used find_one() and pprint to display one document in the establishments collection.
9. Assigned the establishments collection to a variable.


## Part 2: Update the Database

Completed the following tasks for updating the database:

1. Inserted the supplied data for the "Penang Flavours" restaurant into the establishments collection.
2. Performed a query to find the BusinessTypeID for "Restaurant/Cafe/Canteen" and returned only the BusinessTypeID and BusinessType fields.
3. Updated the "Penang Flavours" document with the correct value for BusinessTypeID.
4. Performed a query to delete all the documents in the collection where "Dover Local Authority" was the value for LocalAuthorityName.
5. Conducted a count_documents() check before and after the removal of the Dover documents to ensure the documents were removed.
6. Used update_many() query to convert the latitude and longitude fields from strings to decimal numbers and RatingValue to integers.

## Part 3: Exploratory Analysis

Completed the following tasks for the exploratory analysis:

Question 1: Found establishments with a hygiene score equal to 20. Used count_documents() to list the correct number of documents (answer: 41). Printed the first result using pprint and converted the results to a Pandas DataFrame, displaying the first 10 rows.
Question 2: Found establishments in London with a RatingValue greater than or equal to 4. Used count_documents() to list the correct number of documents (answer: 33). Printed the first result using pprint and converted the results to a Pandas DataFrame, displaying the first 10 rows.
Question 3: Found the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours". Printed all five results using pprint and converted the results to a Pandas DataFrame, displaying.
Question 4: Determined how many establishments in each Local Authority area have a hygiene score of 0. Sorted the results from highest to lowest and printed out the top ten local authority areas. Used an aggregation pipeline to include a match query, group, and sort. Printed the first ten results using pprint and converted the results to a Pandas DataFrame, displaying.
