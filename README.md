# Food Magazine Ratings Analysis

## Overview
In this project, ratings data from a food magazine were analyzed to assist journalists and food critics in determining where to focus future articles. The analysis involved setting up a NoSQL database, updating the database with new information, and performing exploratory data analysis to answer specific questions.

## Project Specifications
### Part 1: Database and Jupyter Notebook Set Up
1. **Database Setup**: Imported data from the establishments.json file into MongoDB, creating a database named uk_food and a collection named establishments.

2. **Library Import**: Imported necessary libraries such as PyMongo and Pretty Print (pprint) in the Jupyter Notebook.

3. **Mongo Client**: Created an instance of the Mongo Client to interact with the MongoDB database.

4. **Database Confirmation**: 
   - Listed databases to confirm uk_food was created.
   - Listed collections to ensure establishments was present.
   - Displayed one document from the establishments collection using find_one and pprint.

### Part 2: Update the Database
1. **Add New Restaurant**: Added information for a new halal restaurant, Penang Flavours, to the establishments collection with a NewRatingPending status.

2. **Find BusinessTypeID**: Found the BusinessTypeID for "Restaurant/Cafe/Canteen" and returned the BusinessTypeID and BusinessType fields.

3. **Update Restaurant**: Updated the new restaurant Penang Flavours with the BusinessTypeID found.

4. **Remove Establishments**: Checked the number of documents containing the Dover Local Authority, removed establishments within Dover, and verified the deletion.

5. **Data Type Conversion**: 
   - Converted latitude and longitude values to decimal numbers using update_many.
   - Converted RatingValue to integer numbers using update_many.

### Part 3: Exploratory Analysis
1. **Question 1**: Identified establishments with a hygiene score equal to 20.

2. **Question 2**: Identified establishments in London with a RatingValue greater than or equal to 4.

3. **Question 3**: Identified the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score and nearest to the new restaurant, Penang Flavours.

4. **Question 4**: Determined the number of establishments in each Local Authority area with a hygiene score of 0, sorted the results from highest to lowest, and printed out the top ten local authority areas.

## Code Source
This code was authored by Lauren Ables-Torres and edX Bootcamps, LLC.
