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

#### 1. Bank Account Distribution and Percentage 

| Bank Account Status | Count | Percentage (%) |
| :--- | :---: | :---: |
| **No** | 20,058 | 85.89% |
| **Yes** | 3,296 | 14.11% |
| **Total** | **23,354** | **100.00%** |

Out of 23,354 total individuals in the dataset, **85.89%** (20,058 individuals) do not have a bank account, 
while the remaining **14.11%** (3,296 individuals) do.


#### 1.3 Bank Account Ownership

![Bank Account Ownership Distribution](https://github.com/user-attachments/assets/719b8874-df7b-4dfa-8297-6d37fed6b9dc)


#### 1.3  Visualization of Bank Account Ownership by Country 

![Bank Account Ownership Distribution](https://github.com/user-attachments/assets/a09bd820-e0fc-4161-96fe-4d61f1e951f2)
#### Key Observations:
* **Overall Trend:** Across all four countries, the number of individuals without a bank account ("No") heavily outnumbers those with a bank account ("Yes").
* **Highest Account Ownership:** **Kenya** shows the highest volume of individuals with a bank account (around 1,500), showing the narrowest gap between the two categories among the countries surveyed.
* **Lowest Account Ownership:** **Uganda** contains the smallest overall sample in this visualization, with the lowest number of banked individuals.
* **Largest Unbanked Population:** **Rwanda** exhibits the highest total number of individuals without a bank account (exceeding 7,500), followed closely by **Tanzania** (nearly 6,000).

####  📈 2.2 Bank Account Rate by Country (%)

| Country | No (%) | Yes (%) |
| :--- | :---: | :---: |
| **Kenya** | 74.94% | 25.06% |
| **Rwanda** | 88.52% | 11.48% |
| **Tanzania** | 90.78% | 9.22% |
| **Uganda** | 91.36% | 8.64% |



#### 2.3 Financial Inclusion Rate by Country (%)
![ Financial Inclusion Rate by Country (%)](https://github.com/user-attachments/assets/9968daa8-e529-4091-878e-85528a1b3b73)

#### Key Takeaways:
* **Kenya** stands out significantly, leading financial inclusion with a **25.06%** bank account ownership rate.
* **Rwanda** sits in the middle with a moderate inclusion rate of **11.48%**.
* **Tanzania** (**9.22%**) and **Uganda** (**8.64%**) register the lowest inclusion levels, both remaining under the 10% threshold.



#### 👥 3.1 Bank Account Ownership by Gender

![Bank Account Ownership by Gender](https://github.com/user-attachments/assets/244412e2-9ddd-4887-b7bd-c1a5c842fd69)


**Key Takeaways**
- Pronounced Unbanked Disparity: The absolute volume of unbanked individuals is significantly higher among females than males, with unbanked females exceeding 12,000 compared to under 8,000 for males.
- Marginal Inclusion Edge: Despite a smaller total sample size in the dataset, males maintain a slight absolute edge in successfully holding a bank account.
- Systemic Gender Gap: This visualization underscores a clear gender-based inclusion gap, highlighting that women face disproportionate socioeconomic or structural barriers to accessing traditional banking systems in East Africa.















