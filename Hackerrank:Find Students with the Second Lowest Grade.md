# 🎓 Hackerrank:Python Program to Find Students with the Second Lowest Grade

This program reads student names and their corresponding grades, identifies the **second lowest grade**, and prints the names of all students who have that grade in **alphabetical order**.

---

## 🎯 Aim

To write a Python program to:
- Read a list of students and their grades.
- Identify the second lowest grade.
- Print the names of students who have that grade, sorted alphabetically.

---

## 🧠 Algorithm

1. **Read** an integer `n` representing the number of students.
2. **Read** each student’s name and grade, and store them as a sublist inside a list.
3. **Extract** all the grades and sort them.
4. **Identify** the second lowest grade from the sorted grade list.
5. **Collect** names of all students whose grade matches the second lowest grade.
6. **Sort** the names alphabetically.
7. **Print** each name on a new line.

---

## 💻  Program
```python
# Number of students
n = int(input("Enter number of students: "))

students = []


for _ in range(n):
    name = input("Enter student name: ")
    grade = float(input("Enter student grade: "))
    students.append([name, grade])

grades = sorted({grade for name, grade in students})
second_lowest = grades[1]


second_lowest_students = [name for name, grade in students if grade == second_lowest]
second_lowest_students.sort()

for student in second_lowest_students:
    print(student)

## Sample Input

5
Harry
37.21
Berry
37.21
Tina
37.2
Akriti
41
Harsh
39

## Output

Harry
Berry

## Result
The program successfully identifies and prints the names of students with the second lowest grade in alphabetical order.

