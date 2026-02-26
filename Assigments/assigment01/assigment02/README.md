**Problem 1 – Student Performance Analytics System**

The purpose of this program is to analyze students’ performance using functions and Object-Oriented Programming (OOP).

**Functions:**

calculate_average(student) → Calculates the student’s average score.

determine_grade(avg_score) → Assigns a grade based on the average score.

top_student(students_data) → Finds the top-performing student.

passed_students(students_data) → Returns the students who have passed in all subjects.

**Class (StudentAnalytics):**

Manages students’ data.

compute_results() → Calculates averages and grades.

get_top_student() → Returns the top student.

get_class_average() → Computes the class average.

get_unique_grades() → Returns distinct grades.

generate_report() → Generates a structured report.

**Advanced Features:**

Identifying students who are consistently improving.

Converting student data into a tabular-like structure for better readability.

**Problem 2 – Course Enrollment & Performance System**

The purpose of this program is to analyze courses and student enrollments using functions and OOP.

**Functions:**

multi_course_students(courses_data) → Returns students enrolled in multiple courses.

courses_with_many_students(courses_data) → Finds courses with more than 2 students.

student_course_count(courses_data) → Returns the number of courses each student is enrolled in.

all_unique_students(courses_data) → Returns all unique students.

**Class (CourseAnalytics):**

Manages course data.

get_multi_course_students() → Returns students enrolled in multiple courses.

get_student_course_count() → Maps each student to the number of courses they are enrolled in.

get_largest_course() → Finds the largest course.

generate_course_report() → Generates a structured report.

**Advanced Features:**

Transforming course-centered data into a student-centered structure.

Data Structure Justification

**Sets (for enrollment)**

Students in courses are stored in sets to prevent duplicate enrollments.

Allows fast membership checks and simplifies analysis of students enrolled in multiple courses.

**Tuples (for fixed scores)**

Student scores are stored in tuples because they are immutable and fixed-length.

Prevents accidental modification of data.

**Dictionaries (for structured mapping)**

Students and courses data are stored in dictionaries for easy access and updates using key-value mapping.

Each student or course can be accessed directly using a unique identifier as the key.

**Classes (for system organization)**

Classes (StudentAnalytics, CourseAnalytics) are used for modularity and encapsulation.

Related functions and data remain organized in one place, making the code readable and reusable. 
