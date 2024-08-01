##### Mouse Tumor Treatment Study
### Overview
This project analyzes data from a study conducted on various drug regimens to observe their effects on tumor volume in mice. The study includes data on different drug regimens, mouse metadata, and study results, including tumor volumes at various time points. The analysis aims to uncover insights into the effectiveness of treatments, potential gender differences, and correlations between mouse weight and tumor size.

### Table of Contents
Project Structure
Data Description
Analysis Steps
Data Preparation
Summary Statistics
Visualizations
Statistical Analysis
Conclusions
How to Run the Code
Dependencies
Author
### Project Structure
bash
Copy code
.
├── Mouse_metadata.csv      # Metadata about the mice used in the study
├── Study_results.csv       # Study results, including tumor volumes
├── analysis.ipynb          # Jupyter Notebook containing the analysis
└── README.md               # Project description and instructions
### Data Description
Mouse_metadata.csv: Contains information about each mouse, including drug regimen, sex, age, and weight.
Study_results.csv: Contains the results of the study, including tumor volumes at various time points and metastatic sites.
### Analysis Steps
## Data Preparation
Merging: The mouse_metadata and study_results datasets were merged based on the Mouse ID.
Data Cleaning: Duplicates were identified and removed. Specifically, entries for mouse ID g989 had duplicate time points.
### Summary Statistics
Generated summary statistics for tumor volumes across different drug regimens, including mean, median, variance, standard deviation, and SEM.
### Visualizations
Bar Charts: Visualized the number of time points for each drug regimen.
Pie Charts: Displayed the distribution of male versus female mice in the study.
Box Plot: Showed the distribution of final tumor volumes for the four most promising regimens (Capomulin, Ramicane, Infubinol, Ceftamin).
Line Plot: Depicted tumor volume over time for a specific mouse treated with Capomulin.
Scatter Plot: Illustrated the relationship between mouse weight and average observed tumor volume for the Capomulin regimen.
Statistical Analysis
Correlation and Regression: Calculated the correlation coefficient and performed linear regression analysis between mouse weight and average tumor volume for the Capomulin regimen.
### Conclusions
Effectiveness: Capomulin and Ramicane were found to be effective in reducing tumor volume.
Gender Balance: The study maintained a balanced representation of male and female mice.
Weight and Tumor Volume: A strong positive correlation was observed between mouse weight and tumor volume in the Capomulin regimen, suggesting a potential biological link.
### How to Run the Code
Clone the repository or download the project files.
Ensure all dependencies are installed (see below).
Open the analysis.ipynb Jupyter Notebook.
Run the notebook cells sequentially to reproduce the analysis and visualizations.
### Dependencies
Python 3.x
Pandas
Matplotlib
SciPy
Jupyter Notebook
Ensure all dependencies are installed using the following:

bash
Copy code
pip install pandas matplotlib scipy jupyter


