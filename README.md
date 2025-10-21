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
## Output

<img width="319" height="118" alt="image" src="https://github.com/user-attachments/assets/f44edf50-1f34-4db7-9807-a7667d4e31f5" />

---

## **Enhancements**
Jupyter Notebook (Refactored_SDLC_Principles.ipynb): Interactive version of the refactored code

## **Extending the Code**:  Visualizations:

Histograms using matplotlib

•	Added Visualizations: Used matplotlib  to plot histograms and seaborn to plot scatter plots of the Iris dataset.
<img width="373" height="290" alt="image" src="https://github.com/user-attachments/assets/1bfe5b70-3cc6-4cad-b785-fe40fe1d60f0" />

Scatter plots using seaborn
<img width="410" height="314" alt="image" src="https://github.com/user-attachments/assets/116364aa-6069-4892-86cf-ccc6dc541470" />


seaborn
---
## **Prerequisites**
Python 3.7+

Required packages: pip install pandas jupyter matplotlib
---
## **How to Run (Bash)**
Clone the repository: git clone https://github.com/Gr8man07/SDLC_Principle-iris-cleanup-activity.git
cd SDLC_Principle-iris-cleanup-activity
Run the messy script: python SDLC_Principles.py
Run the refactored version: python Refactored_SDLC_Principles.py

##**(Optional) Launch Jupyter Notebook:**
Open Refactored_SDLC_Principles.ipynb and run the cells interactively.
---
##** Acknowledgments**
Iris dataset sourced from the UCI Machine Learning Repository
Thanks to the open-source community for tools like Pandas, Jupyter, Matplotlib, and Seaborn
