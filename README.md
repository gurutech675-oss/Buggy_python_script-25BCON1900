# Student Utilities

A simple Python project that provides utility functions to calculate a student's average marks, check pass status, and assign grades.

## Features

- **Calculate Average:** Calculates the average of a list of marks.
- **Check Passing Status:** Checks whether a mark meets the passing threshold of 40.
- **Grade Assignment:** Assigns a grade based on the student's average.

## Functions

### 1. `calculate_average(marks)`

Calculates the average by adding all marks and dividing the total by the number of marks.

Example:
```python
calculate_average([80, 90, 100])
# Output: 90.0
```

### 2. `is_passing(mark)`

Checks whether a mark is greater than or equal to `PASS_MARK`, which is set to 40.

Examples:
```python
is_passing(40)  # True
is_passing(39)  # False
is_passing(75)  # True
```

### 3. `get_grade(average)`

Returns a grade according to the given average.

| Average | Grade |
|---|---|
| 90 and above | Distinction |
| 60–89 | First |
| 45–59 | Second |
| Below 45 | Fail |

Example:
```python
get_grade(95)  # "Distinction"
get_grade(65)  # "First"
get_grade(50)  # "Second"
```

## Usage

Import the functions from `student_utils.py` and use them in your Python program.

```python
from student_utils import calculate_average, is_passing, get_grade

marks = [80, 90, 100]

average = calculate_average(marks)
print("Average:", average)
print("Passing:", is_passing(average))
print("Grade:", get_grade(average))
```

Output:
```text
Average: 90.0
Passing: True
Grade: Distinction
```

## Run Tests

The project includes `test_student_utils.py`, which tests the functions using Python's built-in `unittest` framework.

Run the tests from your terminal:

```bash
python test_student_utils.py
```

## Project Structure

```text
.
├── student_utils.py
├── test_student_utils.py
└── README.md
```

## Requirements

- Python 3
- No external libraries required.

## Purpose

This project demonstrates basic Python functions, arithmetic operations, conditional statements, and unit testing.
