# # 🔢 Hackerrank:# 🏆 Student Topper Finder

This Python program helps determine the **top-performing student** based on the total marks across five subjects. It uses a dictionary to store each student’s marks and identifies the topper using simple calculations and built-in functions.

---

## 🎯 Aim

To maintain a dictionary of students with their marks in five subjects, calculate their **total marks**, store them in a new dictionary, and identify the **student with the highest total (topper)**.

---

## 🧠 Algorithm

1. **Start** the program.
2. Create a dictionary `student_marks`:
   - Keys → Student names.
   - Values → List of marks in five subjects.
3. Initialize an empty dictionary `total_marks`.
4. Loop through `student_marks`:
   - Calculate the total marks using `sum()`.
   - Store the result in `total_marks`.
5. Use `max()` on `total_marks` to find the student with the highest total.
6. Print:
   - The `total_marks` dictionary.
   - The **topper's name and score**.

---

## 💻 PROGRAM:
```python
student_marks = {
    "Alice": [85, 92, 78, 90, 88],
    "Bob": [79, 85, 82, 87, 90],
    "Charlie": [92, 90, 95, 89, 94],
    "David": [88, 84, 86, 91, 85]
}

total_marks = {}
for student, marks in student_marks.items():
    total_marks[student] = sum(marks)


topper = max(total_marks, key=total_marks.get)

print("Total Marks:", total_marks)
print("Topper:", topper, "with", total_marks[topper], "marks")


## OUTPUT
Total Marks: {'Alice': 433, 'Bob': 423, 'Charlie': 460, 'David': 434}
Topper: Charlie with 460 marks

## RESULT
The program successfully identifies the top-performing student by calculating the total marks from a dictionary of student scores.
