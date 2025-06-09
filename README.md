# ETL Extract Lab – DSA 2040A

**Name:** Levin Ekuam  
**Student ID:** m669913  

## 📌 Project Overview

This repository contains my solution to **DSA 2040A – Lab 3: Practicing Extraction in ETL**.  
The lab demonstrates the two main types of data extraction used in ETL processes:

- **Full Extraction:** Load and display the entire dataset.
- **Incremental Extraction:** Load only new records added since the last extraction.

All code is implemented in Python using pandas within a Jupyter Notebook.

---

## 📁 Repository Contents


---

## ⚙️ Tools Used

- **Python 3.12+**: The primary programming language for the project.
- **pandas**: Used for data manipulation and CSV file handling.
- **Faker**: A library for generating synthetic data to populate the dataset.
- **Jupyter Notebook**: The environment for coding, documenting, and testing the ETL extraction logic.
- **Git/GitHub**: Version control and submission platform.

---

## ▶️ How to Run

Open etl_extract.ipynb in Jupyter.
Run all cells to perform full extraction and simulate incremental extraction.
Dataset used: custom_data.csv

## Files used 
etl_extract.ipynb: Notebook with all ETL logic.
custom_data.csv: Generated dataset.
last_extraction.txt: Timestamp for incremental extraction.
.gitignore: To ignore unneeded files in Git.

## screenshots

![image](https://github.com/user-attachments/assets/f343c350-be8f-411a-b94d-59697c6e3885)
through this we can see that we performed a full extraction and it pulled all 100 rows and then we went on to perform a incremental extraction where it pulled 34 rows since it was last updated

![image](https://github.com/user-attachments/assets/e107c265-6867-4d9c-b54c-fb428746d90d)
we then went on to save the new updated time stamp so that the next time data is pulled it will be pulled from this new date


