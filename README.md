# SDLC_Principle-iris-cleanup-activity
A fun classroom project to clean up messy Pandas code for analyzing the Iris dataset. Turns clunky scripts into reusable, well-documented functions!

Iris Dataset Analysis: Clean Code Classroom Activity

**Overview**
This repository contains a classroom activity demonstrating the importance of writing clean, modular, and maintainable code for data analysis. The task involves performing exploratory data analysis (EDA) on the Iris dataset using Python and Pandas. The activity contrasts a messy, non-modular script with a refactored, production-ready version to teach software engineering best practices.

The code performs the following tasks on the Iris dataset:
•	Load the dataset: Reads the Iris CSV from a URL into a Pandas DataFrame.
•	Calculate average: Computes the mean of the sepal_length column.
•	Find maximum: Identifies the maximum value in the petal_width column.
•	Filter rows: Selects rows where the species column is 'setosa' and displays the first five rows.

**Repository Structure**
•	SDLC_Principles.py: The raw, non-modular script that performs the EDA tasks without functions or error handling.
•	Refactored_SDLC_Principles.py: The refactored, clean version with modular functions, error handling, type hints, and documentation.
•	README.md: This file, providing an overview and instructions.
•	iris_analysis.ipynb (optional): A Jupyter Notebook version of the refactored code for interactive use.

**Learning Objectives**
This activity teaches:
•	Modularity: Breaking code into reusable functions.
•	Reusability: Writing functions that work with any DataFrame or column.
•	Maintainability: Making code easy to extend (e.g., adding new calculations).
•	Scalability: Handling larger datasets or multiple CSVs.
•	Reliability: Adding error handling for robustness.
•	Collaboration: Using docstrings and comments for team clarity.
•	Security/Trust: Validating inputs to prevent crashes.

The messy code illustrates common pitfalls (e.g., lack of structure, no error handling), while the refactored code demonstrates best practices for production-ready data analysis.

**Prerequisites**
•	Python 3.7+
•	Dependencies:
o	pandas: For data manipulation.
o	typing and pathlib (included in Python standard library).
•	Optional (for Jupyter Notebook):
o	jupyter: For running .ipynb files.
o	matplotlib (optional): For visualizations.

**Install dependencies:**
pip install pandas jupyter matplotlib
**Usage**
1.	Clone the Repository:
2.	git clone https://github.com/Gr8man07/iris-dataset-analysis.git
3.	cd iris-dataset-analysis
4.	Run the Messy Code: SDLC_Principles.py
5.	python SDLC_Principles.py
This executes the non-modular script, which loads the Iris dataset and performs the EDA tasks.
6.	Run the Refactored Code: Refactored_SDLC_Principles.py
7.	python Refactored_SDLC_Principles.py
This runs the clean, modular version with error handling and reusable functions.
8.	Run in Jupyter Notebook (optional):
o	Launch Jupyter Notebook:
o	jupyter notebook
o	Open iris_analysis.ipynb and run the cells to interactively execute the refactored code.
o	Alternatively, copy the contents of refactored_code.py into a new Jupyter Notebook.
9.	Expected Output:
10.	Average sepal length: 5.843333333333334
11.	Max petal width: 2.5
12.	
13. 	**First 5 rows where species is 'setosa'**:
14.	                sepal_length  sepal_width      petal_length       petal_width        species
15.	   0                5.1             3.5             1.4               0.2            setosa
16.	   1                4.9             3.0             1.4               0.2            setosa
17.	   2                4.7             3.2             1.3               0.2            setosa
18.	   3                4.6             3.1             1.5               0.2            setosa
19.	   4                5.0             3.6             1.4               0.2            setosa

**Code Details**

**Messy Code (SDLC_Principles.py)**
•	Performs all tasks in a single block.
•	Issues: Non-modular, hard to reuse, no error handling, not scalable, no documentation.
**Refactored Code (Refactored_SDLC_Principles.py)**
•	Functions:
o	load_csv_data(file_path): Loads a CSV into a DataFrame with error handling.
o	calculate_column_average(df, column): Computes the mean of a specified column.
o	find_column_max(df, column): Finds the maximum value in a column.
o	filter_by_category(df, column, value): Filters rows based on a categorical value.

**•	Improvements:**
o	Modular and reusable functions.
o	Error handling for missing files, invalid columns, empty data, and non-numeric data.
o	Type hints for better code clarity.
o	Docstrings for collaboration.
o	Structured under if __name__ == "__main__": for proper module execution.

**Jupyter Notebook (Refactored-Modular_SDLC_Principles.ipynb)**
•	Contains the refactored code split into cells for interactive execution.
•	Optional: Add visualizations (e.g., histograms) using matplotlib.

**Extending the Code**
•	Added Visualizations: Used matplotlib  to plot histograms and seaborn to plot scatter plots of the Iris dataset.
<img width="371" height="290" alt="image" src="https://github.com/user-attachments/assets/c20ceb20-6b89-456f-837f-fc6368ff7157" />

<img width="410" height="314" alt="image" src="https://github.com/user-attachments/assets/4cb7e865-33cc-4c51-a6bb-9f19176a8f84" />

**Acknowledgments**
•	The Iris dataset is sourced from UCI Machine Learning Repository.
•	Thanks to the open-source community for tools like Pandas and Jupyter.


