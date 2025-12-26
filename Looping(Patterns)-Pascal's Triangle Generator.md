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
from math import factorial

def nCr(n, r):
    return factorial(n) // (factorial(r) * factorial(n - r))

rows = int(input("Enter number of rows: "))

for i in range(rows):
    print(" " * (rows - i - 1), end="")
     
    for j in range(i + 1):
        print(nCr(i, j), end=" ")
    print()


## Sample Output
	   1
		1 1
		1 2 1
		1 3 3 1
		1 4 6 4 1
        
## Result
The program successfully generates Pascal’s Triangle with the specified number of rows.

	

