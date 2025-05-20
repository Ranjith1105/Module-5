# Exp.No:22  
## Destructor

---

### AIM  
To write a Python program that performs the addition of two numbers using a parameterized constructor and a destructor to delete the instance of the class.

---

### ALGORITHM

1.Begin the program.

2.Define a class named Addition.

3.Create a parameterized constructor __init__(self, a, b) to initialize two numbers.

4.Define a method add(self) to perform and display the addition of the two numbers.

5.Define a destructor __del__(self) to display a message when the object is deleted.

6.In the main section, create an instance of the class by passing two values.

7.Call the add() method.

8.Delete the object using del to trigger the destructor.

9.End the program.

---

### PROGRAM
Reg no: 212223020021
Name: Ranjith P
```
class Fruits:
# Calling constructor
    def __init__(self):
        print('Fruits created.')
# Calling destructor
    def __del__(self):
        print('Destructor called, Fruits deleted.')
obj = Fruits()
del obj

```

### OUTPUT
![Screenshot 2025-04-28 193423](https://github.com/user-attachments/assets/96d5bec8-a4dc-48ab-88dc-b840b23d03ac)



### RESULT
The program successfully adds two numbers using a parameterized constructor and deletes the instance using a destructor.
