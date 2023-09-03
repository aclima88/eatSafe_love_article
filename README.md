# eatSafe_love_article

## Part 1: Database and Jupyter Notebook Set Up

    1. Imported the data provided in the `establishments.json` file from your my Terminal using `shell mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json`. 
    
        a.Named the database `uk_food` and the collection `establishments`.
        
    2. Imported the necessary modules.
    
    3. Created an instance of MongoClient and assigned the uk_food database to variable db.
    
    4. Reviewed the establihsment collection and documents within it and assigned the collection to a variable named establishments.
    
## Part 2: Update the Database
    
    1. Added a new restaurant 'Penang Flavours' to my establishments collection.
    
    2. Updated the BusinessTypeID for 'Penang Flavours'
    
    3. Located all establishments in Dover and deleted those entries from the establishment collection.
    
    4. Changed all longitude and latitude fields from string to decimal.
    
    5. Changed all RatingValue fields from string to integer.
    
## Part 3: Exploratory Analysis

    ### 1. Which establishments have a hygiene score equal to 20?
    
            a. Found out how many establishments had a hygiene score of 20.
        
            b. Converted that list of establishments into a pandas dataframe.

    ### 2. Which establishments in London have a `RatingValue` greater than or equal to 4?
        
            a. Found all of the establishments with London as their Local Authority that had a RatingValue greater than or equal to 4.
            
            b. Converted that list of establishments into a pandas dataframe.

    ### 3. What are the top 5 establishments with a `RatingValue` rating value of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
    
            a. Searched within 0.01 degree on either side of the latitude and longitude of the new restaurant we had previously added to our collection, 'Penang Flavours' for establishments that had a rating value equal 5 and sorted the results by hygiene score in descending order.
            
            b. Converted that list of establishments into a pandas dataframe.
            
    ### 4. How many establishments in each Local Authority area have a hygiene score of 0?
            
            a. Created a pipeline that: 
                1. Matched establishments with a hygiene score of 0.
                2. Grouped the matches by Local Authority.
                3. Sorted the matches from highest to lowest.
            
            b. Converted that list of establishments into a pandas dataframe.
       
#Notes
1. Marshal Rockafellow and I co-worked on this together and bounced ideas and questions off of each other.
2. I had a tutoring session that I used to also work on this module challange.
3. I used google bard and chatGPT for help with syntax issues.
    
