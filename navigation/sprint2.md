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





# 🍿 Digital Divide Popcorn Hack

**Task:** Propose solutions to fix or reduce the digital divide in our community by leveraging existing initiatives and suggesting additional measures.

**Current Efforts:**  
Many communities are already implementing programs like free public Wi-Fi (e.g., Access 4 All Program in San Diego) and computer skill-building classes in libraries. Municipal broadband plans are also being introduced to improve connectivity in underserved areas.

**Additional Solutions:**  
1. **Subsidized Technology Programs:** Introduce grants or low-interest loans to help low-income households purchase digital devices and affordable internet plans.  
2. **Mobile Technology Hubs:** Establish mobile units that can travel to remote or rural areas to provide temporary internet access and digital literacy workshops.  
3. **Public-Private Partnerships:** Encourage collaborations between local governments, non-profits, and tech companies to invest in upgrading digital infrastructure and expanding broadband access.

**Reflection:**  
These solutions build on current initiatives by addressing affordability and accessibility while fostering community engagement and innovation. By combining technology access programs with mobile digital education centers, communities can ensure that everyone has the tools to participate fully in today’s digital world.






