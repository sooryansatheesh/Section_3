# Section 3: Data Transformation

This repository contains a Jupyter Notebook designed to transform a sales dataset. The notebook performs data transformation tasks including date conversion, grouping, and aggregation. It is best used in Google Colab for optimal performance and ease of use.

## Task Description

The primary goal of this notebook is to transform a dataset provided as a CSV file containing sales data. The dataset includes the following columns: `sale_id`, `product_id`, `quantity_sold`, `sale_date`, and `sale_amount`. The transformation tasks include:

1. Converting the `sale_date` column to a datetime format.
2. Adding a new column `year_month` to group data by year and month.
3. Calculating the total sales amount per product per month.

## Efficiency Improvements

To handle large datasets efficiently, the following techniques are used:

1.**Data Processing in chunks**: The large dataset is divided into appropriate chunks for better memory management.

2. **Optimized Data Types**: Appropriate data types are used for storing data based on the values in each column to reduce memory usage.
   
3. **Parquet Files**: Data is stored and processed using Parquet files, which offer efficient data compression and encoding schemes.
   
4. **Multithreading**: Multithreading is used to increase processing speed, especially during data loading and transformation.

## Getting Started

To get started with this notebook, follow the instructions below.

### Prerequisites

You will need a Google account to use Google Colab. If you don't have one, you can create it [here](https://accounts.google.com/signup).

### How to Use

1. **Download the Notebook**: Download the `Section_3.ipynb` file from this repository to your local machine.

2. **Upload to Google Colab**:
    - Go to [Google Colab](https://colab.research.google.com/).
    - Click on the `File` menu and select `Upload notebook`.
    - Choose the `Section_3.ipynb` file you downloaded earlier and upload it.

3. **Run the Notebook**:
    - The first cell of the notebook generates a CSV file with 1 million records of sales data.
    - Run the cells in the notebook sequentially to generate the dataset and perform the data transformation tasks.
    - Ensure you have the necessary libraries installed. The notebook uses `!pip install <library-name>` commands to install any missing libraries.

### Libraries Used

The notebook uses the following Python libraries:
- `os`
- `pandas`
- `datetime`
- `concurrent.futures`
- `numpy`
- `random`


### Features

- **Data Generation**: Generates a synthetic CSV file with 1 million records of sales data.
- **Date Conversion**: Converts the `sale_date` column to a datetime format.
- **Grouping**: Adds a new `year_month` column to facilitate grouping data by year and month.
- **Aggregation**: Calculates the total sales amount per product per month using efficient data manipulation techniques.
- **Optimized Data Types**: Uses optimized data types to reduce memory usage.
- **Parquet Files**: Utilizes Parquet files for efficient storage and processing.
- **Multithreading**: Implements multithreading to speed up data processing.


### Issues

If you encounter any issues or have any questions, feel free to open an issue in the GitHub repository.

---

I hope you find this notebook useful for your data transformation tasks. Happy coding!

