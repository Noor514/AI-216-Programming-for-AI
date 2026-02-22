
## Program Explanation

### Problem 1 – Student Performance Analytics System
Is program ka purpose **students ki performance analyze** karna hai using functions aur OOP.  

- **Functions:**  
  - `calculate_average(student)` → student ka average score calculate karta hai  
  - `determine_grade(avg_score)` → average ke basis par grade assign karta hai  
  - `top_student(students_data)` → top-performing student find karta hai  
  - `passed_students(students_data)` → wo students return karta hai jinhone har subject me pass kiya  

- **Class (`StudentAnalytics`):**  
  - Students ka data manage karta hai  
  - `compute_results()` → averages aur grades calculate karta hai  
  - `get_top_student()` → top student return karta hai  
  - `get_class_average()` → class ka average nikalta hai  
  - `get_unique_grades()` → distinct grades return karta hai  
  - `generate_report()` → structured report generate karta hai  

- **Advanced Features:**  
  - Consistently improving students identify karna  
  - Student data ko tabular-like structure me convert karna  

---

### Problem 2 – Course Enrollment & Performance System
Is program ka purpose **courses aur student enrollment analyze** karna hai using functions aur OOP.  

- **Functions:**  
  - `multi_course_students(courses_data)` → students enrolled in multiple courses  
  - `courses_with_many_students(courses_data)` → courses with more than 2 students  
  - `student_course_count(courses_data)` → har student ka enrolled course count  
  - `all_unique_students(courses_data)` → all unique students return karta hai  

- **Class (`CourseAnalytics`):**  
  - Course data manage karta hai  
  - `get_multi_course_students()` → students in multiple courses  
  - `get_student_course_count()` → mapping of student → number of courses  
  - `get_largest_course()` → largest course find karta hai  
  - `generate_course_report()` → structured report generate karta hai  

- **Advanced Features:**  
  - Course-centered data ko student-centered structure me convert karna  

---

## Data Structure Justification

**1. Sets (for enrollment)**  
- Courses me students ko sets me rakha gaya taki **duplicate enrollments na ho**  
- Fast membership check aur multi-course student analysis easy hota hai  

**2. Tuples (for fixed scores)**  
- Student scores tuples me rakhe gaye kyunki ye **immutable aur fixed-length** hain  
- Data accidentally change nahi hota  

**3. Dictionaries (for structured mapping)**  
- Students aur courses ka data dictionaries me rakha gaya taki **key-value mapping** se easily access aur update ho sake  
- Har student ya course ka **unique identifier** key ke through directly access hota hai  

**4. Classes (for system organization)**  
- Classes (`StudentAnalytics`, `CourseAnalytics`) use ki gayi for **modularity aur encapsulation**  
- Related functions aur data ek jagah organized rehte hain, code readable aur reusable banta hai    