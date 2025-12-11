📊 Vehicle Dataset – Comprehensive Data Analysis

A complete end-to-end data cleaning, exploration, and visualization project on a vehicle specifications dataset.
This project focuses on understanding car characteristics such as engine power, fuel type, vehicle style, size, make/model popularity, and more through effective data preprocessing and EDA.

🧾 Project Overview

This project performs an in-depth analysis on a vehicle dataset containing features like:

Make & Model

Engine HP & Cylinders

Fuel Type

Transmission Type

Driven Wheels

Market Category

Vehicle Size & Style

Year

Number of Doors

The goal is to clean the dataset, transform inconsistent values, visualize key insights, and understand patterns in vehicle characteristics.

📁 Project Steps
🔹 1. Importing Libraries

Used essential Python libraries such as:

Pandas & NumPy (data handling)

Matplotlib & Seaborn (visualizations)

🔹 2. Loading the Dataset

The dataset is loaded using:
df = pd.read_csv("data.csv")

Basic structural checks performed:

df.head()

df.shape

df.info()

df.isnull().sum()

🧹 Data Cleaning & Preprocessing
✔ Handling Missing Values

Removed missing rows from important columns like:
Engine Fuel Type, Number of Doors, Engine Cylinders, Engine HP

Filled Market Category missing values using the mode

✔ Removing Incorrect or Noisy Data

Dropped duplicate rows

Removed entries where:

Engine Cylinders = 0.0 (invalid)

Number of Doors = 3.0 (uncommon/incorrect)

✔ Cleaning Categorical Columns
🔸 Engine Fuel Type

Merged similar fuel names into simplified groups such as:

premium unleaded, regular unleaded → petrol

Standardizing noisy labels

🔸 Transmission Type

Removed UNKNOWN values

Converted all text to lowercase

Grouped rare values into "other"

🔸 Driven Wheels

Standardized "four wheel drive" → "all wheel drive"

🔸 Market Category

High-cardinality column; reduced categories by keeping only frequent combinations (>50 occurrences)

📊 Data Visualization & Insights

The notebook contains detailed visual analysis using bar plots, histograms, pie charts, line plots, and boxplots.

Key Visuals Include:
🔸 Top Vehicle Manufacturers

Chevrolet dominates the dataset

Followed by Ford, BMW, Nissan, Audi, etc.

🔸 Engine Horsepower Distribution

Shows right-skewed distribution

Most cars fall between 150–300 HP

🔸 Top 10 Vehicle Models

Silverado 1500 leads

F-150, Corolla, and Civic appear frequently

🔸 Driven Wheels Distribution

Pie chart shows:

Front-wheel drive is most common

Rear-wheel less common

AWD moderately common

🔸 Market Category Distribution

Crossover dominates

Luxury categories appear in smaller proportions

🔸 Fuel Type by Vehicle Style

Petrol is the most used

Diesel & electric appear rarely

Hybrid limited to few styles

🔸 Vehicle Size Distribution

Compact cars dominate

Full-size and large are less common

🔸 Engine HP vs Cylinders

Strong positive correlation (more cylinders → more HP)

🔸 Vehicles Over the Years

Year-wise trend plot showing dataset coverage

📘 Tech Stack

Python

Pandas

NumPy

Matplotlib

Seaborn

Jupyter Notebook

🚀 How to Run This Project

Clone or download the project

Install required libraries:

pip install pandas numpy matplotlib seaborn


Run the notebook:

jupyter notebook

🏁 Conclusion

This project showcases strong data cleaning, preprocessing, exploratory analysis, and visualization skills. It demonstrates the ability to handle messy real-world data and derive meaningful insights — ideal for resumes and data analytics portfolios.


Soham Patel
Machine Learning | Deep Learning | GenAI | Computer Vision | Date Analysis