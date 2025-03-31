---
layout: page
title: Sprint 2
description: Sprint 2
hide: false
---
# 📖 Digital Divide Homework Hack

Below is the solution to the Digital Divide homework hack. The code reads the preprocessed dataset, then loops through each row to print the country name, its internet access rate from World Bank data, and a status message depending on whether the rate is above 70% or not.

```
import pandas as pd

# Load the dataset and drop unneeded columns
data = pd.read_csv("internet_users.csv").drop(columns=['Notes', 'Year.2', 'Users (CIA)', 'Rate (ITU)', 'Year.1'])
data_cleaned = data.dropna()  # Remove rows with missing values

# Loop through each row in the cleaned dataset
for index, row in data_cleaned.iterrows():
    country = row['Location']
    rate = row['Rate (WB)']
    # Check the internet access percentage and print corresponding message
    if rate > 70:
        print(f"{country}: {rate}%: doing great")
    else:
        print(f"{country}: {rate}%: Needs improvement")
```