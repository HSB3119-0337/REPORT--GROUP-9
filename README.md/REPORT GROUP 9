import pandas as pd
import matplotlib.pyplot as plt
import numpy as np
import seaborn as sns

# Load the data
file_path = '/content/player_data.csv'
df_nba = pd.read_csv(file_path)

# Function to convert height from feet-inches format (e.g., 6-10) to inches
def height_to_inches(height):
    if isinstance(height, str) and '-' in height:
        feet, inches = height.split('-')
        return int(feet) * 12 + int(inches)
    return None

# Apply the height conversion to the dataset
df_nba['height_inches'] = df_nba['height'].apply(height_to_inches)

# Convert height from inches to centimeters
df_nba['height_cm'] = df_nba['height_inches'] * 2.54

# Plot a histogram of player heights in centimeters
plt.figure(figsize=(8,6))
filtered_data = df_nba['height_cm'].dropna()
plt.hist(filtered_data, bins=15, edgecolor='black')
plt.title('Distribution of Player Heights (in cm)')
plt.xlabel('Height (cm)')
plt.ylabel('Number of Players')
plt.show()
