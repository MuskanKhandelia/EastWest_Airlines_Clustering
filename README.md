# EastWestAirlines Clustering

## Data Description

The dataset `EastWestAirlines` contains information on passengers who belong to an airline’s frequent flier program. For each passenger, the data include information on their mileage history and on different ways they accrued or spent miles in the last year. The primary goal is to identify clusters of passengers with similar characteristics for the purpose of targeting different segments for various types of mileage offers.

### Columns in the Dataset:

- **ID:** Unique ID
- **Balance:** Number of miles eligible for award travel
- **Qual_mile:** Number of miles counted as qualifying for Topflight status
- **cc1_miles, cc2_miles, cc3_miles:** Number of miles earned with different credit cards in the past 12 months. Miles are categorized as follows:
  - 1 = under 5,000
  - 2 = 5,000 - 10,000
  - 3 = 10,001 - 25,000
  - 4 = 25,001 - 50,000
  - 5 = over 50,000
- **Bonus_miles:** Number of miles earned from non-flight bonus transactions in the past 12 months
- **Bonus_trans:** Number of non-flight bonus transactions in the past 12 months
- **Flight_miles_12mo:** Number of flight miles in the past 12 months
- **Flight_trans_12mo:** Number of flight transactions in the past 12 months
- **Days_since_enrolled:** Number of days since enrolled in the flier program
- **Award:** Whether the person had an award flight (free flight) or not

## Problem Statement

Perform clustering (K-means clustering) on the airline's data to obtain the optimum number of clusters. The objective is to group passengers based on their characteristics for targeted mileage offers.

## Analysis Summary

### Steps Taken:

1. **Data Preprocessing:**
   - Loaded the dataset and inspected its structure.
   - Checked for missing values and handled them if necessary.

2. **Exploratory Data Analysis:**
   - Explored the distribution of key features.
   - Visualized relationships between variables.

3. **Model Building:**
   - Applied K-means clustering algorithm to identify clusters in the data.
   - Used MinMaxScaler to standardize the data.
   - Utilized the Elbow Method to find the optimal number of clusters (k).

4. **Model Evaluation:**
   - Assessed the model performance using the Within-Cluster Sum of Squares (WCSS).
   - Obtained the inertia value as 324.26.

5. **Results:**
   - Identified cluster means for interpretation and segmentation.
