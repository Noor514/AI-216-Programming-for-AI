
**Overview of Tasks**

This lab focuses on writing structured and modular Python programs using functions and classes.

**Task 1: Data Cleaning Functions**

Implemented functions to:

Remove invalid sensor readings (values below 0 or above 100)

Calculate the average of cleaned data

**Task 2: Student Record Processor**

Developed reusable functions to:

Calculate the average marks of each student

Determine pass/fail status (average ≥ 50)

Display a structured summary for each student

**Task 3: Simple Dataset Class**

Created a class that:

Stores numeric data as an attribute

Returns the number of data points

Calculates and returns the dataset average

**Task 4: Rule-Based Classifier**

Designed a classifier class that:

Stores a threshold value

Classifies individual values as True/False

Classifies a list of values based on the threshold

**Task 5 (Optional): Modular Data Analysis Pipeline**

Combined functions and classes to:

Clean raw numeric data

Store cleaned data inside a class

Compute summary statistics using class methods

**Design Decisions**

Used functions to separate data processing logic into reusable components.

Applied modular design principles to avoid long, single-script implementations.

Designed classes with clear responsibilities, where each class manages its own data and related behavior.

Ensured readability through meaningful function names and structured code organization.

**Challenges Faced**

Deciding how to properly divide logic between functions and classes

Managing data flow between functions and object methods

Ensuring methods correctly accessed and modified internal class attributes

Debugging logical errors while maintaining modular structure
