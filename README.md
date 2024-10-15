                                   INTRODUCTION TO DATA SCIENCE
                                                            -Lecturer:EMANUELPLAN

                                    REPORT-GROUP 9 :TOPIC BASKETBALL 

  ![](images/nab2.jpg)  
  

 I.INTRODUCTION 
  -The dataset "NBA Players Stats since 1950" is sourced from Kaggle, a well-known platform for data science competitions and datasets. It contains detailed statistical 
    data for NBA players, starting from the 1950s to recent seasons. The dataset includes various player performance metrics like points per game, assists, rebounds, shooting 
    percentages, and more. Its purpose is to provide analysts and researchers with a comprehensive view of player performances across different eras of NBA history, enabling 
    comparisons and trend analysis over time
                                                          import pandas as pd
                                                          import numpy as np
                                                          import matplotlib.pyplot as plt
                                                          import pandas
                                                          import statsmodels.api as sm
                                                          import seaborn as sns
                                                          # drive.mount('/content/drive')
                                                          players = pd.read_csv('../input/nba-players-stats/player_data.csv')
