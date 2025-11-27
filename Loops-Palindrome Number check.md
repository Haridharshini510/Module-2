## Loops in Python: Palindrome Number Checker

## 🎯 Aim
To write a Python program that checks whether a given number is a **palindrome** using loops.

## 🧠 Algorithm
1. Get input from the user and assign it to a variable `num`.
2. Assign the value of `num` to a temporary variable `temp`.
3. Initialize a variable `rev` to 0 (used to store the reversed number).
4. Use a `while` loop to reverse the digits:
   - While `temp > 0`:
     - `rev = (10 * rev) + temp % 10`
     - `temp = temp // 10`
5. After the loop, compare `rev` with `num`:
   - If equal, print that the number is a palindrome.
   - Else, print that it is not a palindrome.

## 🧾 Program
```
num = int(input("Enter a number: "))
temp = num
rev = 0

while temp > 0:
    rev = (rev * 10) + temp % 10
    temp = temp // 10

if rev == num:
    print("The number is a Palindrome")
else:
    print("The number is not a Palindrome")

```
## Output
<img width="527" height="206" alt="image" src="https://github.com/user-attachments/assets/94c49a60-a786-435a-8896-307042263b0b" />
<img width="559" height="229" alt="image" src="https://github.com/user-attachments/assets/95238db9-b364-4b42-9956-d7742400fe8e" />

## Result
