# Data Visualization Lab 1

## Introduction  
I’m Monica Pasupuleti, and in this lab I applied data visualization, preprocessing, and statistical analysis techniques to a real-world logistics dataset (DTDC shipping records).

## Purpose  
My goal was to explore and understand the DTDC dataset by:
- Visualizing relationships and distributions among key variables  
- Cleaning and preprocessing the data (handling missing values, detecting and removing outliers, reducing and scaling features)  
- Performing statistical analysis to summarize central tendencies, dispersion measures, and correlations  

## Key Insights  
- **Tariff vs. Total Amount:** A clear positive relationship showed that higher tariffs almost always correspond to higher total charges.  
- **Payment Modes:** Cash was the most common payment method. Card payments exhibited tighter clustering, suggesting more consistent transaction sizes.  
- **Tariff Distribution:** The tariff distribution was right-skewed, with a handful of extreme values. I used the IQR method to remove these outliers for a more representative analysis.  
- **Consignment Types:** “Dox” (documents) made up about 60% of shipments, indicating most consignments were paperwork rather than parcels.  

## Challenges & Decisions  
- **Missing Values:** A few “Tariff” entries were missing; I chose to impute with the column mean to retain as much data as possible.  
- **Outlier Removal:** I used the IQR method because it handles skewed distributions robustly and preserved the bulk of the dataset.  
- **Feature Scaling:** To prepare for any future modeling, I applied Min–Max scaling to the tariff values, bringing them into the [0,1] range.  
- **Column Selection:** I dropped uniquely identifying columns (like Pouch No) and other non-informative fields to focus on variables with analytical value.  
