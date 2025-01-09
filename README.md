This repository contains a Jupyter Notebook (p13.ipynb) dedicated to analyzing the World University Rankings dataset. 
The project involves querying data via SQL, processing information with pandas DataFrames, 
and generating a variety of plots (bar charts, scatter plots, pie charts, and regression lines) to gain insights into university performances worldwide.


In Project 13, we continue analyzing world university rankings—expanding upon the data exploration done in previous projects. We focus on the QS World University Rankings data, using it to:

Create and query an SQLite database
Conduct data transformations in both SQL and Python
Generate visualizations (bar, scatter, pie, regression line) to interpret institutional performance
Dataset
Source: TopUniversities.com
File: rankings.json
Download Method: We use a custom download function in the notebook to fetch the rankings.json file from a remote repository.
Note: The notebook automatically downloads the dataset, so you do not need to manually download or store rankings.json in your repo.
Features and Learning Objectives
SQL Queries:

Create tables, insert data, and extract insights using SQL commands.
Utilize aggregate functions (e.g., SUM, COUNT, AVG, MAX).
Data Wrangling with pandas:

Convert JSON data into DataFrames.
Merge, group, and filter data.
Compute new metrics (e.g., Citations per International).
Data Visualization:

Bar plots, horizontal bar plots, scatter plots, and pie charts.
Add regression lines to scatter plots to visualize correlations.
Explore the relationship between variables (e.g., Overall vs. Rank).
Statistical Analysis:

Correlation between various ranking metrics.
Compare different countries and institutions.
Dependencies and Setup
To run this notebook properly, make sure you have the following installed:

Python 3.7+
Jupyter Notebook or JupyterLab
Pandas (e.g., pip install pandas)
NumPy (e.g., pip install numpy)
Matplotlib (e.g., pip install matplotlib)
Requests (e.g., pip install requests)
SQLite3 (built-in with most Python installations, but ensure it’s enabled)
Otter-Grader (if you are following the exact environment from your course)
If you’re not using a pre-configured environment, you can create one using Anaconda or venv:

bash
Copy code
# Example using Anaconda:
conda create -n ranking-env python=3.9
conda activate ranking-env
conda install pandas numpy matplotlib requests
Project Structure
bash
Copy code
.
├── p13.ipynb             # Main Jupyter Notebook for the project
├── public_tests.py       # Testing script (provided by the course)
├── expected_dfs.html     # Reference output for DataFrames
├── p13.py                # Script converted from notebook (via jupytext)
├── <other supporting files>
└── README.md             # This README file
p13.ipynb:
The core project notebook, containing all necessary functions, queries, and visualizations.

public_tests.py:
Contains public test cases used to verify correctness.

expected_dfs.html:
An HTML file showing the expected structure of certain DataFrames.

p13.py:
Auto-generated Python script version of the notebook (helpful for submission or version control).

How to Run
Clone or download this repository:

bash
Copy code
git clone https://github.com/<YourUsername>/p13-world-university-rankings.git
cd p13-world-university-rankings
Install dependencies (see Dependencies and Setup).

Launch Jupyter:

bash
Copy code
jupyter notebook
In your browser, open p13.ipynb.

Run Notebook:

Go to Kernel > Restart & Run All to execute all cells in sequence.
The code will automatically download rankings.json if it’s not already present.
Inspect each cell’s output, especially the plots and DataFrame queries.
Check Outputs:

Verify SQL queries and DataFrame transformations match expected results.
View generated plots for correctness.

Name: N. Wray
Partner: J. Gartner
Email: nwray2l@wisc.edu
Feel free to open a GitHub issue or pull request if you find bugs or have suggestions for improvements.
