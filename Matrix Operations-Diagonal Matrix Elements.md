# Matrix Operations-Diagonal Matrix Elements Printer 

This Python program reads a matrix of any size from the user and prints **only the diagonal elements**, leaving other elements blank in the output.

##  Aim

To write a Python program that prints only the diagonal elements of a given matrix.

##  Algorithm

1. Read the number of rows and columns from the user.
2. Initialize an empty matrix of size `rows × columns`.
3. Populate the matrix with user input.
4. Display the full matrix.
5. Iterate through the matrix and:
   - If `i == j`, print the element (main diagonal).
   - Else, print a blank space.
6. Print a newline after each row.

##  Program
```
# Initialize empty matrix
matrix = []


for i in range(3):
    row = list(map(int, input().split()))
    if len(row) != 3:
        print("Please enter exactly 3 numbers per row.")
        exit()
    matrix.append(row)

# Display the matrix
print("Matrix:")
for row in matrix:
    print(*row)

# Extract Major and Minor Diagonal Elements
major_diagonal = [matrix[i][i] for i in range(3)]
minor_diagonal = [matrix[i][2 - i] for i in range(3)]

# Print the diagonals
print("Major Diagonal Elements : ", *major_diagonal)
print("Minor Diagonal Elements : ", *minor_diagonal)
```
### Output:
<img width="759" height="385" alt="image" src="https://github.com/user-attachments/assets/d50a7846-a0c8-4fb1-9ab1-49120dc5326c" />

## Result
The Program was executed successfully
