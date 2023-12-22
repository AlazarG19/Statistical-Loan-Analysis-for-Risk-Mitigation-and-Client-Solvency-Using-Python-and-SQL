---
jupyter:
  kernelspec:
    display_name: Python 3 (ipykernel)
    language: python
    name: python3
  language_info:
    codemirror_mode:
      name: ipython
      version: 3
    file_extension: .py
    mimetype: text/x-python
    name: python
    nbconvert_exporter: python
    pygments_lexer: ipython3
    version: 3.11.5
  nbformat: 4
  nbformat_minor: 5
---

::: {#bc41cb72 .cell .markdown}
# Statistical Loan Analysis for Risk Mitigation and Client Solvency. {#statistical-loan-analysis-for-risk-mitigation-and-client-solvency}

This project aims to revel trends and patterns that hold the key to more
prudent and sustainable lending decisions.By doing this you can steer
financial professionals towards sound decision making, enhanced risk
assessment and more responsible lending practices.

In the dynamic landscape of financial services, the pursuit of ensuring
responsible lending practices and minimizing risk is a perpetual
mission. Financial institutions navigate a labyrinth of challenges, but
within these challenges lies an exceptional opportunity -- the power of
statistical analysis.

Predicting a client\'s creditworthiness is akin to wielding a key that
unlocks a world of possibilities. It empowers financial institutions to
tailor loan terms with precision, a measure that not only ensures loans
are made on proper terms but also minimizes default rates, benefiting
both clients and the institution. In essence, it\'s a pathway to not
just optimizing lending practices but revolutionizing financial risk
management as a whole.
:::

::: {#561517ad .cell .markdown}
## Objectives

### Analysing Loan Data

Retrieving the data that is stored in the loans.csv file

### Pursuing Data Purity

Cleaning the dataset to address missing, inconsitent and duplicate data

### Data Preparation and Column Transformation

Preparing dataset for analysis by removing any unnecessary columns and
renaming some columns to improve calrity and consistency.

### Optimizing and storing the present data

Applying different optimization techniques such as Categorizing for
efficiency and Archiving the Insights for later use

### Importing Data to Database and Creating Database Conneciton

Importing data to sql inorder to make the analysis.

### Trend Analysis

Identifying and analysing trends in World Bank Loan Distribution over
time and exploring patterins in loan allocation across different regions
and sectors
:::

::: {#be33a45e .cell .markdown}
## Dataset

The dataset, sourced from the loan department provides a detailed
overvies of each loans with their respective description. This datase
encompasses a range of critical information related to loans granted for
diverse projects. THe datset is strucuted with the following columns
:::

::: {#f9008b97 .cell .markdown}
## Tools

We\'ll be using the the library pandas from the python function to
facilitate data manipulation and perform inital assessment of the
dataset\'s strucutre. Once that is complete We\'ll be using mysql to
formulate SQL queries to extract relevant information for trend
analysis.
:::

::: {#a216962b .cell .markdown}
## Approach

### Preparing Our Data

#### Analyzing Loan Data. {#analyzing-loan-data}

By diving into this dataset, we aim to ensure that every loan we extend
is based on thorough statistical evaluation, reducing risk and ensuring
client success. With pandas and Python by our side, we\'re equipped to
turn this raw data into actionable insights, contributing to a brighter
financial future for our clients and our institution.

#### Pursuing Data Purity. {#pursuing-data-purity}

We tackle the task of identifying and eliminating duplicates within our
loan records. We undertake this mission to ensure the accuracy and
reliability of our financial data. By pinpointing and removing
duplicates, we create a clean and uncluttered dataset, reducing the risk
of erroneous decisions and enhancing our ability to provide clients with
transparent and trustworthy financial services.

#### Removing Duplicates for Precision Lending. {#removing-duplicates-for-precision-lending}

By eliminating duplicates, we aim to create a streamlined and error-free
database that underpins our commitment to responsible lending. Each
duplicate erased ensures that our clients\' financial journeys are free
from confusion and ambiguity.

#### Addressing Null Values. {#addressing-null-values}

We focus on identifying and rectifying null values within our loan
dataset. We undertake this task to ensure that our financial records are
complete and reliable. By addressing null values, we aim to provide a
comprehensive and trustworthy dataset, enabling more precise lending
decisions.

#### Ensuring Data Completeness

By removing null values, we aim to provide a dataset that\'s reliable
and comprehensive, thereby facilitating well-informed lending decisions

#### Renaming Columns for Clarity

We\'ve embarked on a task to rename columns within our loan dataset. We
undertake this mission to enhance the readability and understanding of
our data. By assigning more intuitive and informative column names, we
aim to facilitate smoother data analysis and interpretation.

#### Categorizing for Efficiency. {#categorizing-for-efficiency}

We\'re working on categorizing specific columns within our loan dataset.
We\'ve taken on this task to optimize data storage and speed up data
processing. By converting selected columns into categorical data types,
we aim to reduce memory usage and accelerate data analysis.

#### Archiving the Insights. {#archiving-the-insights}

We\'re executing a task to save our loan dataset in a CSV file. We
ensure that our valuable insights and lending history are securely
stored, facilitating easy retrieval and analysis. Once that\'s done we
can convert it into an sql file using various tools and continue to our
trend analysis. Helpful sites include
<https://tableconvert.com/csv-to-sql>. This has been my tool for
converting my csv to sql effortlessly

### Trend Analysis {#trend-analysis}

Once we\'ve prepared our data, we\'ll use sql to analyse any patterns
with the data

#### Data Download, Import, and Database Connection. {#data-download-import-and-database-connection}

We\'ll start by loading sql libraries and connecting to the sql. In
order to load the data we\'ll have to use MySQLWorkbench. we\'ll first
login into our Local instance. Once that is complete, we\'ll have to
create a new schema to hold our new table. after the schema is created,
use the table data import wizard to load the data into the csv. During
the import, MYSQL Workbench will prompt the data type of each dataset.
During this process, select the appropriate data types such as datetime
, double , string to the needed attributes.Alternatively you can use my
approach by converting the csv to sql then importing it as sql.

### Key Things to Consider and Explore

#### Glimpse into the World of Loans. {#glimpse-into-the-world-of-loans}

We execute a simple yet essential task -- counting the records. We
undertake this mission to gain insights into the scale of our lending
operations and the volume of data at our disposal. By counting the
records, we obtain a clear picture of our dataset\'s size and potential.

#### Profiling Loan Data. {#profiling-loan-data}

We perform this mission to gain a deeper understanding of interest rates
and loan amounts. By selecting, counting, and aggregating specific data
points within a defined interest rate range, we extract valuable
statistics. Each calculated metric sheds light on the lending landscape,
offering us a comprehensive view of interest rate dynamics and loan
amount variations.

#### Navigating Loan Metrics.¶ {#navigating-loan-metrics}

We aim to extract valuable insights into the interest rates and loan
amounts within a specific range. By calculating statistics like loan
count, average interest rate, and loan amount extremes, we gain a
comprehensive understanding of our lending practices.

#### Charting the Loan Landscape. {#charting-the-loan-landscape}

We embark on a task to group and count loans based on their duration and
status. By employing SQL to organize this data, we uncover patterns and
trends within our loan portfolio. The grouped data allows us to better
understand the distribution of loans across different durations and
statuses. This insight supports more informed decision-making and
strategic planning, helping us tailor our lending offerings to align
with the needs of our clients.

#### Employability and Interest Rates. {#employability-and-interest-rates}

We perform this task to identify how employment influences borrowing
costs and to understand the distribution of loans among different
employment categories. Through SQL\'s grouping and aggregation, we gain
insights into average interest rates across various employment statuses.

#### Homeownership and Interest Rates. {#homeownership-and-interest-rates}

We undertake this mission to discern how owning a home impacts borrowing
costs and to assess the distribution of loans among homeowners and
non-homeowners. By utilizing SQL to group and aggregate this data, we
gain insights into average interest rates for these distinct groups.

#### Unpacking Prosper Ratings. {#unpacking-prosper-ratings}

We embark on this task to uncover how creditworthiness influences
borrowing costs and to understand the loan distribution across different
Prosper rating categories. Through SQL\'s grouping and aggregation, we
extract insights into average interest rates for each rating category.

#### Loan Amounts and Monthly Payments. {#loan-amounts-and-monthly-payments}

We perform this task to comprehend how the size of loans impacts the
monthly financial commitment for borrowers. By using SQL\'s grouping and
aggregation, we gain insights into the average monthly payments for
various loan amount categories.

#### Examining Interest Rates and Lending Dynamics. {#examining-interest-rates-and-lending-dynamics}

We undertake this mission to unravel how investor involvement influences
borrowing costs and to gain a better understanding of the loan
distribution across various investor scenarios. By employing SQL\'s
grouping and aggregation, we extract insights into the average interest
rates associated with different levels of investor participation.

#### Loan Durations and Return Rates. {#loan-durations-and-return-rates}

We embark on this task to comprehend how the duration of loans impacts
the returns for investors, and to assess the distribution of loans
across different timeframes. Through SQL\'s grouping and aggregation, we
gain insights into the average return rates for loans of varying
durations.

#### Prosper Ratings and Return Rates. {#prosper-ratings-and-return-rates}

We undertake this task to understand how creditworthiness influences the
investment returns for our stakeholders and to evaluate the distribution
of loans across different Prosper rating categories. Utilizing SQL\'s
grouping and aggregation, we extract insights into the average return
rates for each rating category.
:::
