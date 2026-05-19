# 📊Financial-Inclusion-Analysis-in-East-Africa

### 🌍 Project Overview


- This project analyzes financial inclusion in East Africa using survey data from Kenya, Rwanda, Tanzania, and Uganda to understand factors influencing bank account ownership.
- It explores socio-economic and demographic patterns to identify barriers to financial access in the region.

### 1️⃣ Problem Statement
Problem Statement:
- Financial inclusion plays an important role in economic growth and poverty reduction. 
Despite this, many individuals in East African countries such as Kenya, Rwanda, Tanzania, and Uganda still lack access to formal banking services.
- This project is about to  analyze socio-economic and demographic factors affecting bank account ownership using data from 23,524 individuals, with the goal of identifying the key barriers to financial inclusion in East Africa.


### 2️⃣ Project Objectives
Main Objective:
- To analyze the factors influencing financial inclusion and bank account ownership among individuals in East Africa.
Specific Objectives:
- To understand and explore the Financial Access in East Africa dataset.
- To identify the key socio-economic and demographic factors affecting access to bank accounts.
- To compare financial inclusion patterns across Kenya, Rwanda, Tanzania, and Uganda.


### 3️⃣ Data Source 
- The dataset used in this project is the Financial Access in East Africa dataset, obtained from survey data collected across four East African countries: Kenya, Rwanda, Tanzania, and Uganda.

- The dataset contains socio-economic and demographic information used to analyze financial inclusion and access to bank accounts in East Africa.
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


#### 1.4  Visualization of Bank Account Ownership by Country 

![Bank Account Ownership Distribution](https://github.com/user-attachments/assets/a09bd820-e0fc-4161-96fe-4d61f1e951f2)
#### Key Observations:
* **Overall Trend:** Across all four countries, the number of individuals without a bank account ("No") heavily outnumbers those with a bank account ("Yes").
* **Highest Account Ownership:** **Kenya** shows the highest volume of individuals with a bank account (around 1,500), showing the narrowest gap between the two categories among the countries surveyed.
* **Lowest Account Ownership:** **Uganda** contains the smallest overall sample in this visualization, with the lowest number of banked individuals.
* **Largest Unbanked Population:** **Rwanda** exhibits the highest total number of individuals without a bank account (exceeding 7,500), followed closely by **Tanzania** (nearly 6,000).

####  📈 2.1 Bank Account Rate by Country (%)

| Country | No (%) | Yes (%) |
| :--- | :---: | :---: |
| **Kenya** | 74.94% | 25.06% |
| **Rwanda** | 88.52% | 11.48% |
| **Tanzania** | 90.78% | 9.22% |
| **Uganda** | 91.36% | 8.64% |



#### 2.2 Financial Inclusion Rate by Country (%)
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



#### 3.2 Cell Phone Access IN East Africa 

![Image](https://github.com/user-attachments/assets/c49c66e0-cb4f-41d3-8182-85b3e8534fb6)


**Key Takeaways**

- High Overall Access: Across the region, significantly more people have cell phone access than those who do not.

- Rwanda Leads: Rwanda has the highest number of individuals with cell phone access, exceeding 7,000.

- Tanzania's Gap: Tanzania has the highest number of people without cell phone access compared to the other nations.


#### 3.4 Bank Account Ownership According To The Level Of Education

![Bank Account Ownership According To The Level Of Education](https://github.com/user-attachments/assets/ef4dc18d-02ef-45eb-acfe-868d363da01a)
  


**Key Takeaways**

- Education Level Predicts Inclusion: Bank account ownership rates scale heavily with higher education; it is nearly non-existent for individuals with no formal education, but reaches roughly a 50% split for those with tertiary education.

- Massive Unbanked Base in Primary/Secondary Education: The largest volume of unbanked individuals is heavily concentrated in the "Primary education" segment (exceeding 11,000) followed by "Secondary education."

- Vocational and Tertiary Parity: "Vocational/Specialised training" and "Tertiary education" are the only categories where the number of individuals with a bank account matches or exceeds the number of those without one.

### 3.5 Relationship Between Type of Job and Bank Account Ownership


![Relationship Between Type of Job and Bank Account Ownership](https://github.com/user-attachments/assets/ae097187-bc04-48cc-bcd9-4efead5458f2)


**Key Takeaways**

Formal Employment Highest Penetration: "Formally employed Government" and "Formally employed Private" are the only sectors where bank account ownership ("Yes") meets or exceeds the unbanked population.

Massive Informal Sector Gap: The largest volumes of unbanked individuals are heavily concentrated in informal roles, specifically "Self employed" (over 5,500), "Informally employed" (around 5,000), and "Farming and Fishing" (nearly 5,000).

Vulnerable Groups Lack Access: Categories dependent on alternative cash flows—such as "Remittance Dependent," "Other Income," and "No Income"—show critically low levels of traditional bank account ownership.


### 9️⃣ Recommendations

- Central Banks & Financial Regulatory Authorities: To implement the tiered KYC (Know Your Customer) frameworks and relax documentation requirements for low-income or rural individuals.

- Commercial Banks & FinTech Companies: To design the cash-flow-driven micro-savings/credit products and build the inclusive, low-literacy user interfaces.

- Telecommunication Companies (Telcos): To partner with banks on seamless, low-cost mobile wallet interoperability, bridging the gap between cell phone ownership and bank account access.

- International Development Agencies & NGOs: To fund and deploy the gender-intentional financial literacy programs and micro-grants aimed at closing the gender gap.

- Ministries of Finance & Economic Planning (of Kenya, Rwanda, Tanzania, and Uganda): To integrate these financial inclusion strategies into national development goals for poverty reduction and economic growth.










