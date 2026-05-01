# dhs-sis-analysis
Student Information System (SIS) — Degree Audit Analysis
A data analysis project that simulates a degree audit system for the Dominican House of Studies (DHS). Using Python and Pandas, this project explores student enrollment data to answer key academic advising questions.
Overview
This project works with four datasets:

Students — student IDs and their enrolled program
Courses — course names, categories, and credit values
Program Requirements — required credits per category for each degree
Enrollments — courses taken by each student, with grades and completion status

The programs analyzed include STB, MA Theology, Master of Divinity, MA Thomistic Studies, STL, and STD.
Pipeline

Merge student, course, and enrollment data
Filter for valid courses (completed with a grade ≥ 2.0)
Aggregate credits by student and category
Compare against program requirements
Compute graduation progress and eligibility
Identify missing required categories per student
Analyze course difficulty by grade and completion rate

Questions Answered
1. Who is eligible to graduate?
Built a graduation eligibility checker that compares each student's completed credits against their program's category requirements. Computed a Graduation_Progress score per student reflecting their overall completion percentage.
2. Which students are missing required categories?
Since the dataset reflects mid-program enrollment rather than students near graduation, I pivoted to a more actionable question — identifying students who have zero credits in a required category. This is useful for advisors who need to know who to reach out to before it's too late.
3. What courses are most difficult or easy?
Analyzed courses by average grade and completion rate to surface patterns in course difficulty. Used a 2x2 framework (high/low grade × high/low completion) to interpret results and flag courses that may need curricular review.
Tools Used

Python
Pandas
Google Colab

Author
Karl Ocampo
kvrlwho@berkeley.edu
