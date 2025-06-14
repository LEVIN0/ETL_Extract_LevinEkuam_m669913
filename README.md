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

---

## 🔄 Data Transformation (Lab 4 Update)

This update extends the ETL pipeline with data transformation logic. Transforming the full and incremented dataset

l was able to save the incremented data into its own csv file to help with the lab
![image](https://github.com/user-attachments/assets/33d59127-b92c-4be7-91c8-29a97571ecd0)


### ✅ Transformations Applied

1. **Cleaning**
   - checking for duplicates and missing values if any and removing them
     ![image](https://github.com/user-attachments/assets/264b793b-f525-468a-bc88-602941cc17d5)
     ![image](https://github.com/user-attachments/assets/6adaa1f8-586c-446b-a746-fef2a9df0d1c)

     there were no duplicates and missing values in the dataset as shown in the images above 



2. **Enrichment**
   - Added a new column `total_price` which computes the price of the product * quantity to show the amount used by the customer
   - Added a column called `customer_type` which classifies the customer to either VIP for spending more than 1000 or regular for spending less than 1000
   - ![image](https://github.com/user-attachments/assets/3943df68-98cc-498e-bf77-abf123cf8f3e)
   - ![image](https://github.com/user-attachments/assets/d17acd81-32f2-4a49-9bda-00fc5dd66515)



3. **Structural**
   - this is to ensure that all the columns of the dataset are of the required type and to change where it is not
   - ![image](https://github.com/user-attachments/assets/17a936df-3402-48f8-bcff-2c51f14ddc53)

   - ![image](https://github.com/user-attachments/assets/bb3bee4d-c23c-46bb-8ef2-dcce678e3c96)
   -  since all the columns of both datasets were of the right type, no change was made


### 📁 New Output Files

- `transformed_full.csv`: Cleaned and enriched full dataset
- `transformed_incremental.csv`: Cleaned and enriched incremental dataset



