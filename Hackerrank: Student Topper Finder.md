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
```
amount=25000
discount_percentage=5
cst_percentage=2
discount_amount=(discount_percentage/100)*amount
cst_amount=(cst_percentage/100)*amount
final_amount=amount+cst_amount-discount_amount
print(final_amount)
```
## OUTPUT

<img width="1183" height="190" alt="image" src="https://github.com/user-attachments/assets/17e2e2e8-1a19-4e35-b2b8-90535b79f63e" />

## RESULT
The program successfully identifies the top-performing student by calculating the total marks from a dictionary of student scores.
