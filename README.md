# SDLC_Principle-iris-cleanup-activity
A fun classroom project to clean up messy Pandas code for analyzing the Iris dataset. Turns clunky scripts into reusable, well-documented functions!

Iris Dataset Analysis — SDLC Cleanup Activity

##  Overview

This project demonstrates the importance of writing clean, modular, and maintainable code for data analysis using the Iris dataset. It contrasts a messy, monolithic script with a refactored, production-ready version to teach software engineering best practices in Python and Pandas.

---

## Learning Objectives

- **Modularity**: Break code into reusable functions  
- **Reusability**: Write functions that generalize across datasets  
- **Maintainability**: Make code easy to extend and debug  
- **Scalability**: Prepare code for larger datasets or multiple files  
- **Reliability**: Add error handling for robustness  
- **Collaboration**: Use docstrings and comments for clarity  
- **Security/Trust**: Validate inputs to prevent crashes

---

## Repository Structure
├── SDLC_Principles.py # Messy, non-modular script
├── Refactored_SDLC_Principles.py # Clean, modular version with functions and error handling
├── Refactored_SDLC_Principles.ipynb # Optional Jupyter Notebook version
└── README.md # Project documentation


---

## Tasks Performed

- Load the Iris dataset from a URL into a Pandas DataFrame  
- Calculate the average of the `sepal_length` column  
- Find the maximum value in the `petal_width` column  
- Filter and display the first five rows where `species == 'setosa'`

---

## Code Comparison

### Messy Code (`SDLC_Principles.py`)
- All logic in a single block  
- No functions, error handling, or documentation  
- Difficult to reuse or scale

###  Refactored Code (`Refactored_SDLC_Principles.py`)
- Modular functions:
  - `load_csv_data(file_path)`
  - `calculate_column_average(df, column)`
  - `find_column_max(df, column)`
  - `filter_by_category(df, column, value)`
- Includes:
  - Error handling for missing files, invalid columns, empty data
  - Type hints and docstrings
  - `if __name__ == "__main__"` structure for safe execution

---

##  Output

```text
Average sepal length: 5.843333333333334
Max petal width: 2.5

## **First 5 rows where species is 'setosa'**:
   sepal_length  sepal_width  petal_length  petal_width species
0          5.1          3.5           1.4          0.2  setosa
1          4.9          3.0           1.4          0.2  setosa
2          4.7          3.2           1.3          0.2  setosa
3          4.6          3.1           1.5          0.2  setosa
4          5.0          3.6           1.4          0.2  setosa

## **Enhancements**
Jupyter Notebook (Refactored_SDLC_Principles.ipynb): Interactive version of the refactored code

## **Extending the Code**:  Visualizations:

Histograms using matplotlib

•	Added Visualizations: Used matplotlib  to plot histograms and seaborn to plot scatter plots of the Iris dataset.
<img width="371" height="290" alt="image" src="https://github.com/user-attachments/assets/c20ceb20-6b89-456f-837f-fc6368ff7157" />

Scatter plots using seaborn
<img width="410" height="314" alt="image" src="https://github.com/user-attachments/assets/4cb7e865-33cc-4c51-a6bb-9f19176a8f84" />

seaborn

## **Prerequisites**
Python 3.7+

Required packages: pip install pandas jupyter matplotlib

## **How to Run (Bash)**
Clone the repository: git clone https://github.com/Gr8man07/SDLC_Principle-iris-cleanup-activity.git
cd SDLC_Principle-iris-cleanup-activity
Run the messy script: python SDLC_Principles.py
Run the refactored version: python Refactored_SDLC_Principles.py

##**(Optional) Launch Jupyter Notebook:**
Open Refactored_SDLC_Principles.ipynb and run the cells interactively.

##** Acknowledgments**
Iris dataset sourced from the UCI Machine Learning Repository
Thanks to the open-source community for tools like Pandas, Jupyter, Matplotlib, and Seaborn







