<strong><em><h1> Project #3: Determining the Promising Tariff for a Telecom Company</h1>


## Task

Conduct preliminary analysis of Megaline's "Smart" and "Ultra" tariff plans using data from 500 Megaline customers. Analyze customer demographics, location, chosen tariff plans, and the number of calls and messages sent in 2018. Determine which tariff plan yields higher revenue. This analysis will inform marketing and pricing decisions for Megaline.


**Data Description**

- **users** (User Information):
  - `user_id`: Unique user identifier
  - `first_name`: User's first name
  - `last_name`: User's last name
  - `age`: User's age (years)
  - `reg_date`: Tariff activation date (day, month, year)
  - `churn_date`: Tariff termination date (if missing, the tariff was active at the data extraction time)
  - `city`: User's city of residence
  - `tariff`: Tariff plan name

- **calls** (Call Information):
  - `id`: Unique call number
  - `call_date`: Call date
  - `duration`: Call duration in minutes
  - `user_id`: User identifier who made the call

- **messages** (Message Information):
  - `id`: Unique message number
  - `message_date`: Message date
  - `user_id`: User identifier who sent the message

- **internet** (Internet Session Information):
  - `id`: Unique session number
  - `mb_used`: Volume of internet traffic used per session (in megabytes)
  - `session_date`: Internet session date
  - `user_id`: User identifier

- **tariffs** (Tariff Information):
  - `tariff_name`: Tariff plan name
  - `rub_monthly_fee`: Monthly subscription fee in Russian rubles
  - `minutes_included`: Number of included minutes per month in the subscription fee
  - `messages_included`: Number of included messages per month in the subscription fee
  - `mb_per_month_included`: Volume of included internet traffic per month in megabytes
  - `rub_per_minute`: Cost per minute of conversation beyond the tariff package (e.g., if the tariff includes 100 minutes of conversation per month, a fee will be charged for minutes beyond that)
  - `rub_per_message`: Cost per message sent beyond the tariff package
  - `rub_per_gb`: Cost per additional gigabyte of internet traffic beyond the tariff package (1 gigabyte = 1024 megabytes)


**Project Performance Plan**

1. **Step 1: Data Inspection**
   - Open the data files and review the general information.
   - Data file paths:
     - `/datasets/calls.csv. Download dataset`
     - `/datasets/internet.csv. Download dataset`
     - `/datasets/messages.csv. Download dataset`
     - `/datasets/tariffs.csv. Download dataset`
     - `/datasets/users.csv. Download dataset`

2. **Step 2: Data Preprocessing**
   - Convert data to the required data types.
   - Identify and rectify any data errors, if present.
   - Explain the errors found and how they were corrected.
   - Note that calls with zero duration are not errors; they represent missed calls and should not be removed.
   - Calculate for each user:
     - The number of calls made and minutes used per month.
     - The number of messages sent per month.
     - The volume of internet traffic used per month.
     - Monthly revenue per user (subtract the free limit from the total calls, messages, and internet traffic; multiply the remainder by the tariff plan rates; add the subscription fee corresponding to the tariff plan).

3. **Step 3: Data Analysis**
   - Describe the behavior of the operator's customers based on the sample.
   - Analyze the monthly usage of minutes, messages, and internet traffic for each tariff.
   - Calculate the mean, variance, and standard deviation.
   - Create histograms to visualize the distributions.

4. **Step 4: Hypothesis Testing**
   - Test the following hypotheses:
     - The average revenue of "Ultra" and "Smart" tariff users differs.
     - The average revenue of users in Moscow differs from users in other regions.
   - Define the alpha threshold.
   - Explain how the null and alternative hypotheses were formulated.
   - Specify the hypothesis testing method used and justify the choice.

5. **Step 5: Write a Conclusion**
   - Format: Perform the task in a Jupyter Notebook.
   - Use code cells for program code and markdown cells for explanations.
   - Apply formatting and headings.


## Used skills and libraries
*pandas* , *python*, *ETL* 
*Matplotlib* , *NumPy* , *SciPy* , *Descriptive Statistics* ,
*Statistical Hypothesis Testing*

