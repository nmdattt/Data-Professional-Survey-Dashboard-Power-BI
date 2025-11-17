# Data Professional Survey Breakdown – Power BI Dashboard

## Overview
This project analyzes a global Data Professional Survey and visualizes key insights about job roles, salaries, countries, skills, and career satisfaction.

Using Power BI, the project covers data cleaning (Power Query), data modeling, KPI creation (DAX), and dashboard storytelling.
The final dashboard helps users understand trends in the data industry and support data-driven career or hiring decisions.

## Dataset
The dataset contains 630 survey responses, including:

* Job title
* Salary (USD)
* Country
* Age
* Preferred programming language
* Education level
* Career switch information
* Happiness ratings
* Difficulty breaking into the data field
* Time taken / time spent answering the survey

## Data Cleaning & Transformation (Power Query)

### 1. Column cleanup & restructuring
* Removed unnecessary columns (multiple stages)
* Duplicated columns for safe transformation
* Reordered columns for better schema organization

### 2. Data splitting (extensive use of Split Column)
* Used several split operations:
    * `Split Column by Delimiter`
    * `Split Column by Character Count`
* Purpose:
    * Extract clean values from multi-response fields
    * Separate combined text fields
    * Normalize values for modeling

### 3. Data type corrections
* Converted column types throughout the cleaning flow:
    * **Numeric** → salary, age, ratings
    * **Text** → country, title, language
    * **Date/time** → time spent, survey timestamp

### 4. Value normalization & replacement
* Performed multiple value corrections:
    * Standardized categories
    * Replaced inconsistent answers
    * Fixed spelling / formatting variations

### 5. Custom transformations
* Used `Added Custom` steps to:
    * Extract new columns
    * Recalculate fields
    * Add logical/derived fields

### 6. Filtering & final cleanup
* Removed rows that do not meet analysis criteria
* Filtered out blanks, invalid entries, or irrelevant categories

## Data Modeling
A clean, analysis-ready model was constructed:

* **Fact table:** survey responses
* **Dimension fields:** job title, country, education, gender, programming language
* Proper data types, hierarchies, and relationships

## KPI Development (DAX)
Key DAX measures created:

* Average Age
* Average Yearly Salary
* Count of Survey Takers
* Difficulty Score
* Happiness with Work–Life Balance
* Happiness with Salary
* KPI gauges (0–10 rating scale)

## Dashboard Highlights

### 1. Geographic Distribution
* Treemap showing respondent count by country
   * USA, India, Canada, UK dominate.

### 2. Salary by Job Title
* Bar chart:
   * Data Scientist highest average salary
   * Data Engineer, Architect follow
   * Analyst & entry-level lowest

### 3. Favorite Programming Language
* Stacked bar chart:
   * Python overwhelmingly preferred
   * R, SQL, JavaScript follow.

### 4. Difficulty Breaking Into Data
* Donut chart reveals:
   * 42.7%: Neither easy nor hard
   * 24.7%: Difficult
   * Very few found it "very easy".

### 5. Happiness Metrics
* Gauge charts:
    * Work–Life Balance: 5.74 / 10
    * Salary: 4.27 / 10
* **Insight:** Salary satisfaction is significantly lower.

## Key Insights
* Python dominates as the primary programming language for all roles.
* Data Scientists earn the highest salaries, confirming technical demand.
* Breaking into data is moderately challenging for most respondents.
* Salary satisfaction (4.27) is significantly lower than work-life balance (5.74).
* Survey takers are fairly young (avg age ~29.9), with a high proportion of career switchers.

## Tools & Technologies
* Power BI
* Power Query (M language)
* DAX
* Excel
* Data modeling
* Dashboard design & storytelling

## How to Use
1.  Download repository
2.  Open `.pbix` file in Power BI Desktop
3.  Refresh if needed
4.  Explore using slicers & interactive features
