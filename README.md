# **Project Title**
Recruitment Survey Data Analysis

# **Project Overview**
This project involved a comprehensive analysis of a recruitment survey dataset. The primary goal was to clean the raw data, explore the demographic composition of the respondents, and extract key insights from the survey questions to understand the workforce's opinions and characteristics.

# **Problem Statement**
The initial dataset was challenging to work with. It contained inconsistent column names, irrelevant data, and a structure that made direct analysis difficult. Specifically, many questions were multi-select, with answers spread across multiple columns labeled with vague or non-descriptive names, such as "Unnamed: 8" and "Unnamed: 18". This structure prevented a quick and easy summary of the survey results.

# **Project Objective**
The main objectives were:
1.  To clean and prepare the raw data for meaningful analysis.
2.  To analyze the demographic distribution of the survey respondents by division, position, generation, gender, and tenure.
3.  To systematically analyze responses to key survey questions.
4.  To perform a deeper analysis by cross-tabulating survey responses with demographic data to uncover potential correlations.
5.  To summarize all findings into a clear and comprehensive report.

## **Data Cleaning and Preparation**
This section outlines the specific steps taken to clean and prepare the raw data:
* **Irrelevant Column Dropping:** We removed columns that were either entirely empty or not relevant to the analysis. These included `Respondent ID`, `Email Address`, `First Name`, `Last Name`, `Custom Data 1`, `Start Date`, `End Date`, and `Unnamed: 8`.
* **Header Row Removal:** The first row of the dataset, which contained descriptive labels like 'Response' and 'Answer', was removed as it was not a data entry and would have interfered with our analysis.
* **Column Renaming:** Key demographic columns were renamed to be more descriptive and easier to work with. The following columns were renamed:
    * `Identify which division you work in.` became `Division`.
    * `Which of the following best describes your position level?` became `Position`.
    * `Which generation are you apart of?` became `Generation`.
    * `Please select the gender in which you identify.` became `Gender`.
    * `Which duration range best aligns with your tenure at your company?` became `Tenure`.
    * `Which of the following best describes your employment type?` became `Employment_Type`.
* **Question Consolidation:** We identified that the survey questions were often spread across multiple columns (e.g., `Question 1` and `Unnamed: 18`). We combined the data from these related columns to analyze each question's responses accurately.

## **Column Dictionary**
The following is a list of the key columns and their descriptions after the data cleaning process:

* **Division:** The professional division or department where the respondent works.
* **Position:** The respondent's professional seniority level (e.g., Staff, Manager, Department Lead).
* **Generation:** The generation to which the respondent belongs (e.g., Generation X, Millennial).
* **Gender:** The gender identity of the respondent.
* **Tenure:** The duration range of the respondent's employment at the company.
* **Employment_Type:** The type of employment (e.g., Full time Employee).
* **Questions:** A series of questions from the survey, with multi-select options combined from related columns (e.g., `Question 1`, `Question 5`, etc.).

## **Key Insights**

* **Division Demographics:** The survey was heavily weighted towards the **Infrastructure**, **Finance**, and **Information Technology** divisions, which together accounted for a majority of the responses.
* **Workforce Seniority:** The company's workforce has a strong foundation of **long-term employees**, with over 32% having a tenure of 10 or more years. The majority of respondents were **Staff-level** employees, indicating that the survey reflects a bottom-up perspective.
* **Generational and Gender Distribution:** The workforce is primarily a mix of **Generation X** and **Millennials**, with a fairly balanced gender representation.
* **Diverse Opinions:** For the survey questions analyzed (Q1, Q5, Q6, Q7, Q8), there was no single dominant answer. This suggests a diversity of opinions across the organization rather than a strong consensus on most topics.
* **Correlations with Demographics:** The analysis of Question 6 showed that opinions can differ significantly based on professional seniority. `Chief / Executive` respondents, for example, showed a different response pattern compared to `Staff` and `Managers`, which suggests varying priorities or perspectives based on position. In contrast, for the same question, responses were largely consistent across different gender groups.

## **Overall Insight**

The overall insight is that this data reveals a stable, mature workforce with a diverse range of opinions. While some demographic groups share similar perspectives, there are notable differences based on seniority, as seen in the analysis of Question 6. The lack of a strong consensus on most questions indicates that a one-size-fits-all approach to company policies may not be effective, and more targeted initiatives might be required.

## **Conclusion**

We have successfully processed and analyzed the recruitment survey data, transforming a complex and unorganized dataset into a valuable source of information. The insights gathered about demographics and employee opinions provide a solid foundation for further decision-making. The project highlights the importance of data cleaning and systematic analysis to uncover meaningful trends. The next steps could involve analyzing the remaining questions or conducting a deeper dive into specific correlations to inform strategic initiatives within the company.
