# 📊Financial-Inclusion-Analysis-in-East-Africa

### 🌍 Project Overview


This project analyzes financial inclusion in East Africa using survey data from Kenya, Rwanda, Tanzania, and Uganda to understand factors influencing bank account ownership.
It explores socio-economic and demographic patterns to identify barriers to financial access in the region.

### 1️⃣ Problem Statement
Problem Statement:
Financial inclusion plays an important role in economic growth and poverty reduction. 
Despite this, many individuals in East African countries such as Kenya, Rwanda, Tanzania, and Uganda still lack access to formal banking services. T
his project seeks to analyze socio-economic and demographic factors affecting bank account ownership using data from 23,524 individuals, with the goal of identifying the key barriers to financial inclusion in East Africa.


### 2️⃣ Project Objectives
Main Objective

To analyze the factors influencing financial inclusion and bank account ownership among individuals in East Africa.
Specific Objectives
To understand and explore the Financial Access in East Africa dataset.
To identify the key socio-economic and demographic factors affecting access to bank accounts.
To compare financial inclusion patterns across Kenya, Rwanda, Tanzania, and Uganda.


### 3️⃣ Data Source 
The dataset used in this project is the Financial Access in East Africa dataset, obtained from survey data collected across four East African countries: Kenya, Rwanda, Tanzania, and Uganda.

The dataset contains socio-economic and demographic information used to analyze financial inclusion and access to bank accounts in East Africa.
Download the dataset from Kaggle [download here the dataset](https://www.kaggle.com/datasets/sarahmabrouk/financial-inclusion-in-africa)

### 4️⃣ Variables / Dataset Features

| Variable | Description |
|---|---|
| Country | Country of the respondent |
| Age of respondent | Respondent's age |
| Gender of respondent | Male/Female |
| Marital status | Current marital status |
| Education level | Highest education attained |
| Job type | Employment category |
| Location type (Urban/Rural) | Residential area classification |
| Cell phone access | Whether the respondent owns/accesses a phone |
| Relationship with head of household | Family relationship status |
| Year | Year of data collection |
| Unique ID | Identifier for each respondent |


### 5️⃣ Tools Used
#### Python 
- NumPy
- Pandas
- Seaborn
- Matplotlib

### 6️⃣ 🧹 Data Cleaning

- Removed Invalid Year Values: Incorrect survey years such as 2029, 2039, and 2056 were identified and removed. Only valid survey years (2016, 2017, and 2018) were retained.
- Removed Missing Values: Rows containing missing (NaN) values in important variables were removed to maintain data consistency and reliability.
- Removed Invalid Education Entries: The invalid value "6" was removed.
The category "Other/Dont know/RTA" was also removed because it did not provide meaningful educational information.

### 7️⃣ Data Transformation

- Renamed Columns for Better Readability:
- uniqueid → unique_id
- Has a Bank account → Bank_account
- Type of Location → Location
- Cell Phone Access → Phone_access
- Respondent Age → Respondent_age
- gender_of_respondent → gender
- The relathip with head → Relationship_with_head
- Level of Educuation → Education_level
- Type of Job → job_type


### 8️⃣ Exploratory Data Analysis (EDA)

















