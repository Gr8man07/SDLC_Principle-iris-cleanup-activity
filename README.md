Iris Data Cleanup Activity
A fun classroom project to turn messy Pandas code into clean, reusable functions for analyzing the Iris dataset, complete with cool visualizations!
Overview
This project is all about making code better! It takes a clunky, hard-to-read script for analyzing the Iris dataset and transforms it into a clean, modular, and production-ready version. You’ll see how software engineering principles like modularity and error handling can make data analysis more reliable and fun to work with. Plus, we add visualizations to explore the data visually.
The code:

Loads the Iris dataset from a URL into a Pandas DataFrame.
Calculates the average sepal_length.
Finds the maximum petal_width.
Filters rows where species is 'setosa' and shows the first five.
Visualizes sepal_length as a histogram or scatterplot.

Learning Objectives

Break code into reusable functions (no more giant scripts!).
Write code that works with any dataset.
Make code easy to tweak or debug.
Handle bigger datasets or multiple files.
Add error checks to avoid crashes.
Use comments and docstrings so others can understand your code.
Explore data with visualizations like histograms and scatterplots.

Repository Structure
├── messy_code.py              # Messy, non-modular script
├── refactored_code.py         # Clean, modular version with functions and visualizations
├── iris_analysis.ipynb        # Jupyter Notebook for interactive use
├── README.md                 # This file
└── images/                   # Folder for visualization screenshots
    ├── histogram.png         # Histogram of sepal_length
    ├── scatterplot.png       # Scatterplot of sepal_length vs. sepal_width

Tasks Performed

Load the Iris dataset from a URL.
Calculate the average of the sepal_length column.
Find the maximum value in the petal_width column.
Filter and display the first five rows where species is 'setosa'.
Create a histogram of sepal_length or a scatterplot of sepal_length vs. sepal_width.

Code Comparison
Messy Code (messy_code.py)

All logic in one block.
No functions, error handling, or comments.
Hard to reuse or scale for other datasets.

Refactored Code (refactored_code.py and iris_analysis.ipynb)

Functions:
load_csv_data(file_path): Loads a CSV with error handling.
calculate_column_average(df, column): Computes a column’s mean.
find_column_max(df, column): Finds a column’s maximum.
filter_by_category(df, column, value): Filters rows by a value.


Features:
Error handling for missing files, invalid columns, or empty data.
Type hints and docstrings for clarity.
if __name__ == "__main__": for safe execution.
Visualizations using Seaborn (histogram or scatterplot).



Output
Average sepal length: 5.843333333333334
Max petal width: 2.5

First 5 rows where species is 'setosa':
   sepal_length  sepal_width  petal_length  petal_width  species
0           5.1          3.5           1.4          0.2  setosa
1           4.9          3.0           1.4          0.2  setosa
2           4.7          3.2           1.3          0.2  setosa
3           4.6          3.1           1.5          0.2  setosa
4           5.0          3.6           1.4          0.2  setosa

Visualizations

Histogram of Sepal Length (using Seaborn):
Scatterplot of Sepal Length vs. Sepal Width (using Seaborn, colored by species):

Prerequisites

Python 3.7+
Required packages:pip install pandas seaborn matplotlib jupyter



How to Run

Clone the Repository:
git clone https://github.com/Gr8man07/iris-data-cleanup.git
cd iris-data-cleanup


Run the Messy Code:
python messy_code.py


Run the Refactored Code:
python refactored_code.py


Run in Jupyter Notebook:
jupyter notebook

Open iris_analysis.ipynb and run the cells to see the analysis and visualizations.


Extending the Code

Try Different Visualizations: Modify iris_analysis.ipynb to plot other columns (e.g., petal_length) or use Matplotlib instead of Seaborn.
Add More Stats: Create functions for median, minimum, or standard deviation.
Use Other Datasets: Update the file_path in load_csv_data to analyze a different CSV.

Troubleshooting

ModuleNotFoundError: Ensure all packages are installed (pip install pandas seaborn matplotlib jupyter).
Internet Issues: If the Iris URL fails, download the CSV locally and update file_path.
Visualization Issues: Check that seaborn and matplotlib are installed and that you’re running in a graphical environment (e.g., Jupyter).
Jupyter Not Opening: Try jupyter notebook --no-browser --port=8888 and open the provided URL.

License
MIT License. See LICENSE for details.
Acknowledgments

Iris dataset from UCI Machine Learning Repository.
Thanks to Pandas, Seaborn, Matplotlib, and Jupyter for awesome tools!





