# Important Note
Submission branch is **main** branch. The develop branch is for work, so please refer to the main branch.

# Predicting U.S. Weekly Business Applications 
Udacity Data Scientist Nanodegree – Course 2 Project


## Motivation
- Weekly business application counts are a leading indicator of economic activity.
Policy makers and entrepreneurship support organizations need timely insights beyond quarterly reports.
Using the U.S. Census Bureau’s Business Formation Statistics (Weekly Data), this project aims to build a model that predicts the next week’s total U.S. non-seasonally adjusted business applications (BA_NSA).

- Why this topic?

    - Quarterly data can lag behind rapid market changes.

    - Weekly trends help stakeholders make faster, data-driven decisions

## Environment

- **Python**: 3.10 or higher  
- **Required Libraries (as seen in requirements.txt)**:  
    - numpy
    - pandas
    - scikit-learn
    - matplotlib

## Getting Started and Reproducing the Analysis
1. Fork and Clone the repository
```bash
git clone https://github.com/<your-handle>/udacity-datascientist-course2.git
cd udacity-datascientist-course2
```

2. (Optional) Create a virtual environment
```bash
python -m venv venv
source venv/bin/activate          # For Windows: venv\Scripts\activate
```

3. Install dependencies
```bash
pip install -r requirements.txt
```

4. Reproducing the analysis
    Launch Jupyter 
    ```bash
    jupyter notebook
    ```

    Open project_course2.ipynb → Run all cells (Kernel → Restart & Run All).

## File Overview
```bash
├── data/  
│   ├── bfs_state_apps_weekly_nsa.csv     # Raw weekly state-level counts  
│   └── bfs_weekly_data_dictionary.pdf    # Official data dictionary  
├── project_course2.ipynb             # Main Jupyter Notebook (CRISP-DM workflow) 
├── requirements.txt                      # Reproducible Python environment  
└── README.md
```

## Summary of Results
| Model | RMSE | MAE |
| ------- | ------- | ------- |
| Linear Trend (days only) | 25502 | 22045 |
| Linear Regression (multi) | 8852 | 5612 |
| Decision Tree | 7517 | 4707 |

## License, Author & Acknowledgments
- Author: Takumi Matsubara
- Acknowledgments:
    - Data provided by U.S. Census Bureau (Business Formation Statistics)
        - https://www.census.gov/econ/bfs/data/weekly.html
    - A non-technical summary and discussion of findings is available on Medium:  
        - https://medium.com/@takumi.matsubara/reading-the-pulse-of-american-entrepreneurship-48fa572341d9
