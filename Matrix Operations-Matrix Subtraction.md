
##  AIM:
Write a Python Program  to  find the product of two matrices. Check the condition to multiply two matrices, if the condition is false, print "Cannot Multiply"

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

---

##  PROGRAM:
```
def read_matrix(r,c):
    matrix = [[0]*c for row in range(r)]
    for i in range(r):
        lines = list(map(int, input().split()))
        for j in range(c):
            matrix[i][j] = lines[j]
    return matrix
def print_matrix(M):
    print("Matrix:")
    for i in range(len(M)):
        for j in range(len(M[0])):
            print(M[i][j],end=" ")
        print()
def product(M,N):
    C=[[0]*len(N[0]) for i in range(len(M))]
    for i in range(len(M)):
        for j in range(len(N[0])):
            for k in range(len(N)):
                C[i][j] = C[i][j]+M[i][k]*N[k][j]
    return C
r1,c1=input().split()
M=read_matrix(int(r1),int(c1))
r2,c2=input().split()
N=read_matrix(int(r2),int(c2))
if(c1==r2):
    print_matrix(M)
    print_matrix(N)
    R=product(M,N)
    print_matrix(R)
else:
    print("Cannot Multiply")
```

## OUTPUT:
<img width="601" height="759" alt="image" src="https://github.com/user-attachments/assets/a5175a91-4868-4974-8254-f6dd6a519d93" />

## RESULT:
The Program was executed successfully
