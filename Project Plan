# Project Plan: IT PM Project 1

## 1. Course Name

IT Project Management

## 2. Team Information

- **Team Name:** SOLO TEAM
- **Group:** I24B

**Team Members**

- **Team Leader:** Ra'no Botirova | Student ID: 202490090 | Group: I24B | Role: Project Manager | Phone: +998330040545

## 3. Project Title

**IELTS Online Learning Platform: Website Development**

## 4. Dataset Information

- **Dataset Title:** IELTS Student Learning and Progress Dataset
- **Source Website / URL:** [Existing IELTS Course Website](https://english-course.ielts9.workers.dev/)
- **Description of the Dataset:** The dataset will contain sample student information, course enrollment records, practice results for Reading and Listening, Writing and Speaking assessment scores, payment records, and learning progress.
- **Why This Dataset Was Selected:** The data will help us understand students' learning performance, identify frequently used features, monitor progress across all four IELTS skills, and examine course enrollment and payment trends.
- **Size of Dataset (rows, columns):** To be determined after the sample dataset is created.

**Data source note:** The existing website is the reference system for our project. We will use synthetic or manually prepared sample data for analysis unless actual data is made available with appropriate authorization. We will not assume access to the website's private student records.

## 5. Project Objectives

### Problem Statement

The existing demonstration website is the starting point for our project. Our proposed system aims to expand its learning functionality by creating a new website which will include  Writing and Speaking alongside Reading and Listening, as well as introducing an online payment system.

Students should be able to access IELTS learning materials and practice activities through one platform, while the system can organize their learning progress and course access.

### Main Objectives

1. Upgrade the existing demonstration website by creating a new, more complete IELTS learning platform.
2. Provide practice and learning resources for all four IELTS skills: Reading, Listening, Writing, and Speaking.
3. Implement online payment functionality for course enrollment or access.
4. Provide a student dashboard for viewing learning activities and progress.
5. Analyze sample student performance and enrollment data using Python and Pandas.
6. Evaluate the usability, functionality, and reliability of the proposed system.

### Questions to Answer Through Data Analysis

- Which IELTS skill has the lowest average practice score?
- How does student performance vary across the four skills?
- Which courses or learning modules receive the most enrollments?
- Is there a relationship between practice activity and student performance?
- What proportion of sample payment transactions are successful or unsuccessful?

### Expected Insights

The analysis is expected to identify students' weaker IELTS skills, reveal patterns in practice activity and course demand, and demonstrate how learning and payment data could support better platform management. These are expected outcomes, not confirmed findings.

## 6. Data Preparation Using Pandas

We will prepare a sample dataset for analysis using Python and the Pandas library.

### A. Loading the Dataset

We will store sample learning records in a CSV file and load them into Python.

```python
import pandas as pd

df = pd.read_csv("ielts_student_data.csv")

print(df.head())
print(df.info())
```

This allows us to inspect the dataset's structure and data types.

### B. Cleaning the Data

We will check for missing values, duplicate records, incorrect data types, and invalid score values.

```python
print(df.isnull().sum())
print(df.duplicated().sum())

df = df.drop_duplicates()
```

Missing values will be handled according to the meaning of each field rather than automatically replacing all of them.

### C. Data Transformation and Feature Creation

We will standardize column names, validate IELTS practice scores, and calculate an average score across the four skills where the required values are available.

```python
skills = ["reading", "listening", "writing", "speaking"]

df["average_skill_score"] = df[skills].mean(axis=1)
```

The average will be calculated only when the necessary skill scores are present, with missing values handled according to the chosen analysis rules.

## 7. Data Analysis Tasks Using Pandas

We will use Pandas to analyze the prepared dataset.

### A. Filtering and Sorting

Identify students whose average practice scores are above a selected threshold.

```python
high_performers = df[
    df["average_skill_score"] >= 7.0
]

print(high_performers)
```

This identifies records meeting the chosen threshold; it does not establish an official IELTS band score.

### B. Grouping and Aggregation

Calculate average performance across the four IELTS skills.

```python
skill_averages = df[skills].mean()

print(skill_averages)
```

This helps us identify which skill has the lowest average score in the sample.

### C. Enrollment Analysis

Count enrollments by course or learning module.

```python
enrollment_counts = df.groupby(
    "course_name"
).size().sort_values(ascending=False)

print(enrollment_counts)
```

This helps identify the most frequently selected courses in the sample.

### D. Payment Analysis

Examine the number of transactions by payment status.

```python
payment_summary = df.groupby(
    "payment_status"
).size()

print(payment_summary)
```

This will help demonstrate how payment records can be monitored in the proposed system.

### E. Visualization

We will create charts to compare average skill scores, course enrollment counts, and payment statuses. The charts will help present the results clearly in the final report and presentation.

## 8. Key Findings and Insights

The final findings will be completed after the dataset has been prepared and analyzed.

We expect to investigate:

- Which IELTS skills need more practice based on the sample results.
- Which courses or learning modules are most popular.
- How students' practice activity relates to their scores.
- Whether payment records reveal transaction problems in the sample.

The findings will be used to explain how data analysis can help improve course planning, student support, and platform management. No numerical findings will be reported until the analysis is completed.

## 9. Project Timeline (5 Weeks)

The following is a proposed five-week schedule. The original template's September–October dates and October 14 presentation date should be confirmed with the instructor because those dates have passed.

| Week | Activities |
|---|---|
| Week 1 | Project planning, existing website review, requirements gathering, and scope definition |
| Week 2 | UI/UX design, database planning, sample dataset creation, and data cleaning |
| Week 3 | Website development, four-skill learning modules, payment workflow design, and initial Pandas analysis |
| Week 4 | Integration, system testing, data visualization, bug fixing, and documentation |
| Week 5 | Final testing, project report, diagrams, presentation preparation, and demonstration |

**Presentation Date:** To be confirmed with the instructor.

## 10. Outcome of the Project

By completing this project, students are expected to:

- Understand the stages of IT project planning and system development.
- Practice gathering requirements and defining project scope.
- Design a database and organize a website's main functions.
- Understand how online learning and payment workflows operate.
- Develop skills in Python and Pandas for preparing and analyzing sample data.
- Improve teamwork, testing, documentation, and presentation skills.

The planned deliverables include a website prototype, database design, project documentation, use case diagram, Business Process Model (BPM), Entity Relationship Diagram (ERD), and SQL scripts.

## 11. Conclusion

This project aims to upgrade an existing IELTS learning website into a more complete online learning platform. By adding Writing and Speaking practice, online payment functionality, and student progress monitoring, the proposed system will bring important learning activities together in one place.

Pandas analysis of sample learning and payment records will complement the system development work by demonstrating how data can support educational decisions and platform management. The project will also provide practical experience in requirements analysis, system design, development planning, testing, and teamwork.

## 12. References

1. Existing IELTS Course Website: https://english-course.ielts9.workers.dev/
2. Pandas Documentation: https://pandas.pydata.org/docs/
3. Python Documentation: https://docs.python.org/3/
4. Official IELTS Website: https://ielts.org/
5. Course materials and guidelines provided for IT Project Management.

## 13. Appendix

The appendix will include:

- Important Python and Pandas code snippets.
- The sample dataset and its data dictionary.
- Charts showing student performance and course enrollment.
- Use case diagram.
- Business Process Model (BPM).
- Entity Relationship Diagram (ERD).
- Database tables and SQL scripts.
- Website screenshots and testing results.
