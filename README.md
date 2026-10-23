# San-Francisco-Salaries-Analysis-using-Pandas

An exploratory data analysis of San Francisco city employee compensation (2011-2014) using Python and pandas. The notebook answers 21 practical questions that cover data inspection, cleaning, filtering, and aggregation.

# Dataset
-- Source: San Francisco Salaries dataset (public city employee compensation records, available on Kaggle)
-- Size: 148,654 rows x 13 columns
-- Years covered: 2011-2014
# Key columns: EmployeeName, JobTitle, BasePay, OvertimePay, OtherPay, Benefits, TotalPay, TotalPayBenefits, Year


# What the Notebook Covers
- Area	Tasks
- Data inspection	head, tail, shape, info, describe, null-value check
- Data cleaning	Dropping unused columns (Id, Notes, Agency, Status), converting BasePay to numeric, replacing "Not provided" with NaN, dropping   rows with multiple missing values
- Filtering and search	Job titles containing "Captain", Fire Department employees, lookup of a specific employee's pay and job title
- Aggregation	Min/max/mean BasePay, average BasePay per year and per job title, top 5 most common jobs and employee names
Key Findings
- The dataset has 148,654 records, and Notes is completely empty, so it was dropped.
- Benefits has about 36,000 missing values and Status has about 110,000.
- Average BasePay is roughly $66,325, with a maximum of $319,275 (Chief of Police, 2013).
- Average BasePay rose from about $63.6K in 2011 to about $69.6K in 2013, then dipped to about $66.6K in 2014.
- Transit Operator is the most common job title (7,036 records), followed by Special Nurse and Registered Nurse.
- Several columns (BasePay, OvertimePay, OtherPay, Benefits) load as text because of "Not Provided" entries, so they need numeric conversion.
