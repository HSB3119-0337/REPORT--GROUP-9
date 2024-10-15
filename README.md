                                   INTRODUCTION TO DATA SCIENCE
                                                            -Lecturer:EMANUELPLAN

                                    REPORT-GROUP 9 :TOPIC BASKETBALL 

  ![](images/nab2.jpg)  
  

 INTRODUCTION 
  -The dataset "NBA Players Stats since 1950" is sourced from Kaggle, a well-known platform for data science competitions and datasets. It contains detailed statistical data for NBA
    players, starting from the 1950s to recent seasons. The dataset includes various player performance metrics like points per game, assists, rebounds, shooting 
    percentages, and more. Its purpose is to provide analysts and researchers with a comprehensive view of player performances across different eras of NBA history, enabling 
    comparisons and trend analysis over time

                  (CODE)

  PLAYER SET CREATION
                
                  
                  players['career_length'] = players['year_end'] - players['year_start']
                  players.head(10)
                 
                  (CODDE)
              
              Then we can make all of the columns that will be used for analysis
    
        name: The name of the player.
        
        year_start: The starting year of the player's career or the year they began playing in the dataset.
        
        year_end: The ending year of the player's career or the year they stopped playing in the dataset.
        
        position: The positions that players typically occupy, with percentages indicating the proportion of players in each position
       
        height: The height of players, categorized into ranges (e.g., 6-7, 6-8) with the percentage indicating how many players fall into 
             each range.
       
        weight: The weight of players, possibly indicating distribution across different weight ranges.
        
        birth_date: The birth dates of players, with a histogram showing how many players were born in specific years.
        
        college: Indicates the colleges that players attended, with a percentage showing the proportion of players from a specific college 
           
HEIGHT ISSUES

    In the data set, the height vector was set up in the format 'feet-inches' which means a height of 70 inches would read '6-10' as 6 feet 
    ten inches. Since this makes calculations more difficult, I have written the following code to convert these values to the equivalent 
    numbers in inches.

                                  (add code)

                  
                                                         
