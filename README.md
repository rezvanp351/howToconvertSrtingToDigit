# Age Input Validation Program

This simple Python program continuously asks the user to enter their age until they provide a valid numeric input.  
It demonstrates the use of a **`while True` loop**, **input validation**, and **conditional statements** in Python.

---

## 🧠 Features
- Ensures the input is **not empty**.  
- Accepts **only numeric values**.  
- Displays clear error messages for invalid input.  
- Determines whether the user is an **adult** or **under 18**.

---

## 🧩 Code Explanation

```python
while True:
    age_input = input("Enter your age: ").strip()
    
    if age_input == "":
        print("Age cannot be empty. Please enter a number.")
        continue  # repeat the loop
    
    if age_input.isdigit():
        age = int(age_input)
        break
    else:
        print("Invalid input. Please enter a numeric value.")

if age >= 18:
    print("You are an adult.")
else:
    print("You are under 18.")
