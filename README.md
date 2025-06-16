README: Netflix Viewer Engagement Dataset
------------------------------------------------------------------------

Author: Yashitta Bawa
Date of Submission: 16 June 2025
Contact: ybaw0002@student.monash.edu

------------------------------------------------------------------------

1. Data Overview

This project explores viewer engagement patterns on Netflix using two publicly available datasets. The analysis investigates how genres, content format (TV vs movie), and duration relate to total watch hours globally.

Data Sources:

i) Netflix Engagement Report (Jan–Jun 2023)
  -   Type: Observational
  -   Source: https://about.netflix.com/en/news/what-we-watched-a-netflix-engagement-report
  -   Description: Contains global watch hours for titles available on Netflix between January–June 2023. Fields include `title`, `release_date`, and `hours_viewed`.

ii) Netflix Metadata from Kaggle**
  -   Type: Observational
  -   Source: https://www.kaggle.com/datasets/shivamb/netflix-shows
  -   Description: Contains metadata including `title`, `listed_in` (genres), `duration`, `type` (TV or movie), and `release_year`.

These datasets were merged using a cleaned and standardised `title` field.

------------------------------------------------------------------------

2. Files Included

- data/netflix_titles.csv              : Metadata file from Kaggle
- data/Netflix_Engagement_Report.xlsx  : Watch hour data from Netflix
- assignment4_Yashitta_Bawa.qmd        : Main Quarto file (with blog tabs)
- styles.css                           : Custom Netflix-themed stylesheet
- data_description.xlsx                : Data dictionary and variable-level documentation
- README.md                            : This file

------------------------------------------------------------------------

3. How to Use the Data

Both datasets are ready for analysis after basic preprocessing. The `assignment4_Yashitta_Bawa.qmd` file contains all code for merging, cleaning, and visualising the data.

You can use this data for:

- Visualising genre and format trends
- Exploring how duration and show type influence viewership
- Summarising most-watched titles by category

------------------------------------------------------------------------

4. Data Limitations & Considerations

- Coverage: Only includes titles available and watched between Jan–Jun 2023
- Engagement metric: Uses total hours watched, which does not account for viewer drop-off or partial views
- Unit mismatch: `duration` differs by format (minutes for movies, seasons for TV shows); this was resolved using parsed variables
- No individual-level data: No personal, regional, or demographic data is included

All data is fully public and contains no personally identifiable information (PII). Merging and transformation were limited to formatting, type parsing, and genre splitting for analytical purposes.

------------------------------------------------------------------------

5. Ethics and Privacy

This analysis uses public, aggregate-level data. No individual users are represented. There are no ethical risks in merging or transforming this data. The datasets were used strictly for educational and academic analysis under Monash University guidelines.

------------------------------------------------------------------------

6. Citation

- Netflix Engagement Data: 
  Netflix. What We Watched: A Netflix Engagement Report. 
  Retrieved from: https://about.netflix.com/en/news/what-we-watched-a-netflix-engagement-report
- Netflix Metadata: 
  Shivamb. Netflix Movies and TV Shows. Kaggle. 
  Retrieved from: https://www.kaggle.com/datasets/shivamb/netflix-shows

------------------------------------------------------------------------

7. Project Summary

This submission includes all relevant code, documentation, visualisation, and reflections in a modular, reproducible Quarto file. All variables used are clearly documented in `data_description.xlsx`.
