# python-grade-checker
Learning Python through real practice projects — documenting mistakes, improvements, and growth with a goal of joining world-class engineering teams.
# 🚀 Python Learning Journey  

This repository is part of my **personal growth path in Python programming**.  
It contains beginner-friendly projects where I practice concepts, make mistakes, fix them, and share my journey openly.  

My goal is simple: **learn consistently, build step by step, and grow into a world-class software engineer**.  

---

## 📌 Current Project: Student Grade Checker  

This project uses Python’s new **`match-case`** syntax to implement a simple grading system.  
While it looks small, it’s a valuable step in learning how condition handling works in modern Python.  

### 🔹 Features  
- Takes input from the user  
- Applies conditions using `match-case`  
- Outputs grade (A+, A, B, C, Fail)  

---

## 🐞 Issue Faced  

I first wrote the following code:  

```python
n = int(input("Enter your value : "))
print("Your value is : ", n)

match check_num:   # <- This causes an error
    case n if n >= 80 and n < 100:
        print("A+")
    case n if n >= 70 and n <= 80:
        print("Your grade is A")
    case n if n > 60 and n < 70:
        print("Your grade is B")
    case n if n > 50 and n < 60:
        print("Your grade is C")
    case _:
        print("Sorry, Fail")
