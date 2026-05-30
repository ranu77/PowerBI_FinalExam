# PowerBI_FinalExam

📊 Student Performance Dashboard – Academic & Behavioral Insights
A Power BI dashboard built to analyze student academic performance, attendance, and behavior across different classes, subjects, and terms.

📁 Dataset Used
File                                 What it contains
Attendance - Attendance.csv.csv      Date, Status (Present/Absent), Reason
Behavior - Behavior.csv.csv          Date, Behavior Type, Notes
Scores - Scores.csv.csv              Subject, Exam Type, Score, Max Score, Term
Students - Students.csv.csv          Student ID, Name, Gender, Class, Section

🔗 Data Modeling
Connected all 4 tables using StudentID as the common key:
Scores     → Students
Attendance → Students
Behavior   → Students
All relationships are Many to One and Active.

<img width="1305" height="633" alt="image" src="https://github.com/user-attachments/assets/97fe1759-90fe-4654-af57-f54964633517" />

🧹 Data Cleaning

Corrected data types for all columns
Replaced blank values in Reason column with "N/A"

📐 DAX Measures Created
1. % Score
2. Absent Count
3. Attendance %
4. Average Score per Subject
5. Behavior Count
6. Performance Category
7. Total Students

📄 Dashboard Pages

Page 1 — Main Dashboard
-3 KPI Cards — Total Students, Attendance %, Avg Score %
-4 Slicers — Class, Section, Subject, Term
-Bar Chart — % Score by Subject
-Line Chart — % Score by Term
-Table — Student scores with conditional formatting
-Donut Chart — Behavior distribution
-Navigation buttons for Academic and Behavioral views

<img width="1168" height="665" alt="image" src="https://github.com/user-attachments/assets/e7fa2e5c-b606-4859-a347-41a4be041229" />

Page 2 — Academic View

-4 KPI Cards — Total Students, Attendance %, % Score, Performance Category
-2 Slicers — Class, Term
-Bar Chart — % Score by Subject and Class
-Line Chart — Performance trend by Term
-Table — Student scores with Name, Subject, Term, % Score, Performance Category
-Back button

<img width="1165" height="667" alt="image" src="https://github.com/user-attachments/assets/88e404b5-1197-4994-8b01-52ef12bd6b43" />

Page 3 — Behavioral View

-4 KPI Cards — Total Students, Attendance %, Behavior Count, Absent Count
-2 Slicers — Class, Section
-Donut Chart — Behavior types distribution
-Bar Chart — Behavior count by Class and Type
-Table — Behavior log with Name, Type, Date, Notes
-Back button

<img width="1178" height="670" alt="image" src="https://github.com/user-attachments/assets/e765d5f7-1754-4b56-a52e-4fcf01fe240f" />

Page 4 — Student Profile (Drillthrough)

-Drillthrough set on Student Name
-3 KPI Cards — Attendance %, % Score, Performance Category
-1 Slicer — Student Name
-Line Chart — Score trend by Term
-Bar Chart — Score by Subject
-Table — Full score details
-Donut Chart — Behavior breakdown
-Back button

<img width="1170" height="661" alt="image" src="https://github.com/user-attachments/assets/70b4a89a-1a9e-4cb3-a026-08f4bcc3bc10" />






