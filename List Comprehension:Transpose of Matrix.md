
##  AIM:
Write a Python program to print the column-wise sum of a matrix.


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

class Numbers:
    def __init__(self, N=0):
        self.N = int(input())
    def create_list(self):
        self.L=[]
        for i in range(self.N):
            x=int(input())
            self.L.append(x)
    def sorting(self):
        swapped = False
        for i in range(self.N):
            for j in range(0, self.N-i-1):
                if self.L[j] > self.L[j + 1]:
                    swapped = True
                    self.L[j], self.L[j + 1] = self.L[j + 1], self.L[j]
            if not swapped:
                return
    def print_List(self):
        for i in range(self.N):
            print(self.L[i])

```

## OUTPUT:
<img width="689" height="552" alt="image" src="https://github.com/user-attachments/assets/50d33e87-2107-4c00-9567-59f3ae6293fc" />

## RESULT:
The Program was executed successfully



