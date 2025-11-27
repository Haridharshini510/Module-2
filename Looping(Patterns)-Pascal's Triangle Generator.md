# 🔺 Looping(Patterns)-Pascal's Triangle Generator in Python

This project demonstrates a simple Python program to generate **Pascal’s Triangle**, where the number of rows is provided by the user.

---

## 🎯 Aim

To write a Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user.

---

## 🧠 Algorithm

1. Start the program.
2. Input the number of rows from the user.
3. Loop from 0 to the number of rows.
4. For each row:
   - Print appropriate spaces to shape the triangle.
   - Compute values using the formula:  
     \[
     C(n, k) = \frac{n!}{k!(n-k)!}
     \]
5. Print all rows of Pascal’s Triangle.
6. End the program.

---

## 🧪 Program
```
def print_pascals_triangle(rows):
    for i in range(rows):
        print(" " * (rows - i - 1), end="")

        number = 1
        for j in range(i + 1):
            print(number, end=" ")

            number = number * (i - j) // (j + 1)

        print()

rows = int(input())
print_pascals_triangle(rows)
```
## Sample Output
<img width="605" height="603" alt="image" src="https://github.com/user-attachments/assets/07e16570-60a5-43b7-b792-13044865d32f" />

## Result
Thus, the program was executed successfully and Pascal’s Triangle was generated for the given number of rows.

