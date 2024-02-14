# UK Food Standards Analysis with NoSQL

## Overview

In collaboration with "Eat Safe, Love", a renowned food magazine, this project leverages NoSQL databases to analyze food hygiene ratings across the UK. Utilizing MongoDB, a NoSQL database, and Jupyter Notebook for data manipulation and analysis, we aim to provide the magazine's editors with data-driven insights to guide future articles' focus.

### Objective

The primary goal is to explore food hygiene ratings provided by the UK Food Standards Agency, identifying trends and establishments of interest. This analysis will inform "Eat Safe, Love" journalists and food critics on potential highlights and areas of concern, aiding in the decision-making process for future content.

### Methodology

#### Part 1: Database and Jupyter Notebook Setup

- Imported `establishments.json` into a MongoDB database named `uk_food`, creating a collection called `establishments`.
- Utilized PyMongo to interact with the database, confirming successful data import and preparing the collection for analysis.

#### Part 2: Database Update

- Added a new halal restaurant, "Penang Flavours", to the database, enhancing the dataset with current market entries.
- Updated establishment data to ensure accuracy and relevance, including correcting data types for latitude, longitude, and rating values.

#### Part 3: Exploratory Analysis

Focused on answering key questions for "Eat Safe, Love", including:
- Identifying establishments with specific hygiene scores.
- Exploring high-rated establishments in London.
- Analyzing the top 5 establishments near "Penang Flavours" with a rating of 5.
- Assessing hygiene scores across different Local Authority areas.

### Key Findings

- A total of 41 establishments have a hygiene score of 20.
- In London, 33 establishments boast a rating value of 4 or higher.
- The top 5 establishments with a rating of 5, based on proximity to "Penang Flavours", were identified, offering a targeted list for potential reviews.
- Analysis of Local Authority areas revealed significant variations in hygiene scores, highlighting areas for potential improvement and praise.

### Challenges and Solutions

- **Data Import:** Initially, the command used for importing data into MongoDB was omitted. This was rectified by documenting the `mongoimport` command within the Jupyter notebook.
- **Data Accuracy:** Some number values stored as strings were converted to their correct numeric data types to ensure accurate analysis.
- **Query Accuracy:** Adjustments were made to correct the count of establishments in London with a rating value greater than or equal to 4, utilizing regex for precise matching.

### Conclusion

This project underscores the power of NoSQL databases in handling and analyzing large datasets. By providing "Eat Safe, Love" with actionable insights into the food hygiene ratings across the UK, we empower them to make informed decisions on content direction, ultimately enriching their readers' dining experiences.

### Acknowledgments

I extend my gratitude to the editorial team at "Eat Safe, Love" for their collaboration, and to my peers and mentors for their invaluable support throughout this project.
