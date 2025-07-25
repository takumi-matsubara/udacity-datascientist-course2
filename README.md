# udacity-datascientist-cousrse2

## 1. Installation

- **Python**: 3.9 or higher  
- **Required Libraries**:  
    - numpy
    - pandas
    - scikit-learn
    - matplotlib


## 2. Motivation
- Weekly business application counts are a leading indicator of economic activity.
Policy makers and entrepreneurship support organizations need timely insights beyond quarterly reports.
Using the U.S. Census Bureau’s Business Formation Statistics (Weekly Data), this project aims to build a model that predicts the next week’s total U.S. non-seasonally adjusted business applications (BA_NSA).

- Why this topic?

    - Quarterly data can lag behind rapid market changes.

    - Weekly trends help stakeholders make faster, data-driven decisions

## 3. File Overview
- data/
    - bfs_state_apps_weekly_nsa.csv
        - Raw state-level weekly counts. We convert year + week to calendar dates and aggregate to a national series.

    - bfs_weekly_data_dictionary.pdf
        - Definitions and descriptions for each column (including some fields not present in the CSV).

- project_course2.ipynb
    - Jupyter Notebook with data analysis with CRISP-DM step

## 4. License, Author & Acknowledgments
- Author: Takumi Matsubara
- Acknowledgments:
    - Data provided by U.S. Census Bureau (Business Formation Statistics)
        - https://www.census.gov/econ/bfs/data/weekly.html