# Python-Data-Cleaning
A collection of Python-based data cleaning projects. Each project demonstrates essential techniques for preparing raw data for analysis and modeling.

## Introduction
This repository contains Python-based data cleaning projects that demonstrate key steps and best practices for preparing raw data for analysis or modeling. The projects here cover various aspects of data cleaning, such as handling missing values, duplicates, outliers, and ensuring data consistency.

## Project 1: Cafe Sales
### Overview
This project focuses on cleaning a dataset related to cafe sales. The dataset contains information about transactions, including the quantity of items sold, the price per unit, and the total spent.

### Steps Taken
- **Inspecting the Data:** The dataset is loaded and inspected for structure, datatypes, and basic statistics.
- **Handling Missing Values:** Missing values in certain columns (`Payment Method`, `Location`, `Item`) are filled with appropriate values to prevent data loss.
- **Data Type Corrections:** Columns with incorrect data types are converted to appropriate types for analysis.
- **Handling Duplicates:** Duplicate records are removed from the dataset to ensure data integrity.
- **Feature Engineering:** Missing values in `Price Per Unit` and `Total Spent` are imputed based on logical relationships between columns (e.g., calculating `Total Spent` as the product of `Quantity` and `Price Per Unit`).

## Project 2: Customer Care
### Overview
This project focuses on cleaning a customer care dataset. It contains customer details such as contact information, payment status, and preferences for communication.

### Steps Taken
- **Inspecting the Data:** Initial inspection of the dataset is performed to identify data types, missing values, and other issues.
- **Handling Irrelevant Columns:** Irrelevant or unnamed columns are dropped to reduce noise in the data.
- **Cleaning Customer Data:** Columns like `Last_Name` and `Phone_Number` are cleaned by removing special characters, handling missing values, and reformatting phone numbers.
- **Handling Categorical Data:** Missing values in categorical columns (`Paying Customer`, `Do_Not_Contact`) are filled appropriately to ensure consistency in the dataset.
- **Removing Records:** Records where customers have opted out of being contacted are dropped, as well as rows with missing phone numbers.
- **Index Resetting:** The index is reset after data cleaning operations to maintain a clean and continuous index.


## Files Included
### Cafe Sales Project (`Cafe Sales.ipynb`)
- This file contains the code for cleaning the cafe sales data.
- Dataset: Cafe Sales.csv: 
### Customer Care Project (`Customer Care.ipynb`)
- This file contains the code for cleaning the customer care data.
- Dataset: Customer Care.csv

## How to Use
- Clone the repository to your local machine.
- Make sure you have Python 3.x installed along with the necessary libraries: `numpy`, `pandas`.
- Run the `.ipynb` files in Jupyter Notebook or any other compatible Python environment.
- Load the datasets (`Cafe Sales.csv` and `Customer Care.csv`) and follow the steps to clean the data.

## License
This project is licensed under the MIT License - see the LICENSE file for details.