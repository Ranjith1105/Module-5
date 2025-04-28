# Exp.No:25  
## Hierarchical Inheritance

---

### AIM  
To write a Python program to get the employee and doctor details and display them using hierarchical inheritance. Create a parent (base) class named `Details` and two child (derived) classes named `Employee` and `Doctor`.

---

### ALGORITHM

1. **Begin the program.**
2. **Create a class Details** with an `__init__` method to initialize three attributes: `id`, `name`, and `gender`.
3. **Define a method display_details()** to print the values of `id`, `name`, and `gender`.
4. **Create a class Employee** that inherits from the `Details` class. 
   - Add two additional attributes: `company` and `department`.
   - Override the `display_details()` method to print the employee-specific attributes (`company` and `department`) along with the inherited details.
5. **Create a class Doctor** that also inherits from the `Details` class. 
   - Add two additional attributes: `hospital` and `department`.
   - Override the `display_details()` method to print the doctor-specific attributes (`hospital` and `department`) along with the inherited details.
6. **Accept input** for employee and doctor details.
7. **Create objects of Employee and Doctor** using the input.
8. **Call the `display_details()` method** for both objects to print the details.
9. **Terminate the program.**

---

### PROGRAM
Reg no: 212223020021
Name: Ranjith P
```
# Base class
class Details:
    def __init__(self):
        self.name = ""
        self.age = 0

    def get_basic_details(self):
        self.name = input("Enter name: ")
        self.age = int(input("Enter age: "))

    def display_basic_details(self):
        print("Name:", self.name)
        print("Age:", self.age)


# Derived class: Employee
class Employee(Details):
    def __init__(self):
        super().__init__()
        self.employee_id = ""
        self.designation = ""

    def get_employee_details(self):
        self.get_basic_details()
        self.employee_id = input("Enter Employee ID: ")
        self.designation = input("Enter Designation: ")

    def display_employee_details(self):
        self.display_basic_details()
        print("Employee ID:", self.employee_id)
        print("Designation:", self.designation)


# Derived class: Doctor
class Doctor(Details):
    def __init__(self):
        super().__init__()
        self.doctor_id = ""
        self.specialization = ""

    def get_doctor_details(self):
        self.get_basic_details()
        self.doctor_id = input("Enter Doctor ID: ")
        self.specialization = input("Enter Specialization: ")

    def display_doctor_details(self):
        self.display_basic_details()
        print("Doctor ID:", self.doctor_id)
        print("Specialization:", self.specialization)


# Main program
print("--- Enter Employee Details ---")
emp = Employee()
emp.get_employee_details()

print("\n--- Enter Doctor Details ---")
doc = Doctor()
doc.get_doctor_details()

print("\n--- Displaying Employee Details ---")
emp.display_employee_details()

print("\n--- Displaying Doctor Details ---")
doc.display_doctor_details()


```

### OUTPUT  

![Screenshot 2025-04-28 204858](https://github.com/user-attachments/assets/4608b5e8-6607-4321-a412-db79a98e2822)
  


### RESULT
The program successfully demonstrates hierarchical inheritance in Python by collecting and displaying employee and doctor details using a shared base class Details.
