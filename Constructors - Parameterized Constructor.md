# Exp.No:21  
## Constructors - Parameterized Constructor

---

### AIM  
To write a Python program using a class to perform the addition of two numbers using a parameterized constructor.

---

### ALGORITHM

1.Begin the program.

2.Define a class named Addition.

3.Create a parameterized constructor __init__(self, a, b) to initialize two numbers.

4.Define a method add(self) to perform the addition of the two numbers.

5.In the main part of the program, create an object of the class by passing two numbers as arguments.

6.Call the add() method to display the result.

7.End the program.

---

### PROGRAM
Reg no: 212223020021
Name: Ranjith P
```
class Addition:
    first = 0
    second = 0
    answer = 0
     
    # parameterized constructor
    def __init__(self, f, s):
        self.first = f
        self.second = s
     
    def display(self):
        print("First number = " + str(self.first))
        print("Second number = " + str(self.second))
        print("Addition of two numbers = " + str(self.answer))
 
    def calculate(self):
        self.answer = self.first + self.second
 
# creating object of the class
# this will invoke parameterize constructor
x=int(input())
y=int(input())

obj = Addition(x,y)
 
# perform Addition
obj.calculate()
 
# display result
obj.display()


```

### OUTPUT

![Screenshot 2025-04-28 192944](https://github.com/user-attachments/assets/8468e4d2-0020-4935-8258-8a37f3e907f8)

### RESULT
The program successfully performs the addition of two numbers using a class with a parameterized constructor and displays the result.
