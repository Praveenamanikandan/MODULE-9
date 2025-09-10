##  AIM:
Write a Python Program to find whether the given matrix is sparse matrix


---

##  ALGORITHM:
Start

Define the problem to be solved.

Identify the inputs required.

Identify the process/steps needed to solve the problem.

Identify the outputs to be produced.

Write the steps in logical order:

Accept input.

Perform the necessary computations or processing.

Produce and display the output.

Stop

##  PROGRAM:
```

def read_matrix(n):
    matrix = [[0]*n for row in range(n)]
    for i in range(n):
        lines = list(map(int, input().split()))
        for j in range(n):
            matrix[i][j] = lines[j]
    return matrix
def print_matrix(M):
    print("Matrix:")
    for i in range(len(M)):
        for j in range(len(M[0])):
            print(M[i][j],end=" ")
        print()
def check_sparse(M):
    count=0
    for i in range(len(M)):
        for j in range(len(M[0])):
            if(M[i][j]==0):
                count+=1
    if(count > ((len(M)*len(M))//2)):
        print(True)
    else:
        print(False)
n=int(input())
M=read_matrix(n)
print_matrix(M)
check_sparse(M)

```
## OUTPUT:
<img width="350" height="523" alt="image" src="https://github.com/user-attachments/assets/a13a8ebe-0454-4912-8c6e-c98b89fe1b10" />

## RESULT:
The Program was executed successfully
