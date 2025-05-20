# Exp.No:23  
## Multiple Inheritance

---

### AIM  
To write a Python program to get the name, age, and ID of a student and check if they are a valid student using multiple inheritance.

---

### ALGORITHM

1.Begin the program.

2.Create a class Person to get and store the student's name and age.

3.Create another class StudentID to get and store the student ID.

4.Create a derived class Student that inherits from both Person and StudentID.

5.In the Student class, define a method is_valid() to check the following:

       -Name is not empty.
       
       -Age is greater than 0.
       
       -ID is alphanumeric and not empty.
       
6.Create an object of the Student class and input details.

7.Call the is_valid() method to check and print whether the student is valid.

8.End the program.

---

### PROGRAM
Reg no: 212223020021
Name: Ranjith P

```
class Person:  
    #defining constructor  
    def __init__(self, personName, personAge):  
        self.name = personName  
        self.age = personAge  
  
    #defining class methods  
    def showName(self):  
        print(self.name)  
  
    def showAge(self):  
        print(self.age)  
  
    #end of class definition  
  
# defining another class  
class Student: # Person is the  
    def __init__(self, studentpercent):  
        self.studentpercent = studentpercent  
  
    def getpercent(self):  
        return self.studentpercent  
  
  
class Resident(Person, Student): # extends both Person and Student class  
    def __init__(self, name, age, percent):  
        Person.__init__(self, name, age)  
        Student.__init__(self, percent)  
  
  
name=input()
age=int(input())
percent=int(input())
resident1 = Resident(name, age, percent)  
resident1.showName()  
resident1.showAge()  
if resident1.getpercent() > 12000:
    print("Valid Student")
else:
    print("Invalid Student")
    

```

### OUTPUT
![Screenshot 2025-04-28 202923](https://github.com/user-attachments/assets/cb85c5c5-5b9a-471e-9ee3-1fef6b3c8074)



### RESULT
The program successfully collects student details using multiple inheritance and validates them based on name, age, and ID.



