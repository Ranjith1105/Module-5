# Exp.No:24  
## Multi-level Inheritance

---

### AIM  
To write a Python program to get the name, age, and ID of a person and display them using multilevel inheritance.

---

### ALGORITHM

1. Define the `Person` class:
   - Inside the `Person` class, define the `__init__` method (constructor) with two parameters: `name` and `age`.
   - Inside the `__init__` method, assign the `name` to `self.name` and `age` to `self.age`.

2. Define the `PersonDetails` class that inherits from the `Person` class:
   - Inside the `PersonDetails` class, define the `__init__` method (constructor) with three parameters: `name`, `age`, and `person_id`.
   - Inside the `__init__` method, call the `__init__` method of the `Person` class using `super()` to initialize `name` and `age`.
   - Assign `person_id` to `self.person_id`.

3. Define the `DisplayDetails` class that inherits from the `PersonDetails` class:
   - Inside the `DisplayDetails` class, define the `__init__` method (constructor) with three parameters: `name`, `age`, and `person_id`.
   - Inside the `__init__` method, call the `__init__` method of the `PersonDetails` class using `super()` to initialize `name`, `age`, and `person_id`.

4. Inside the `DisplayDetails` class, define the `show_details` method:
   - Inside the `show_details` method, return a formatted string with `self.name`, `self.age`, and `self.person_id`.

5. Prompt the user to enter `name` (string), `age` (integer), and `person_id` (integer).

6. Create an instance `person` of the `DisplayDetails` class, passing `name`, `age`, and `person_id` to the constructor.

7. Call the `show_details` method on the `person` object and print the result.

8. Terminate the program.

---

### PROGRAM
Reg No: 212223020021
Name: Ranjith P
```
# Base class
class Person:
    def __init__(self):
        self.name = ""

    def get_name(self):
        self.name = input("Enter name: ")

    def display_name(self):
        print("Name:", self.name)


# Derived class from Person
class Age(Person):
    def __init__(self):
        super().__init__()
        self.age = 0

    def get_age(self):
        self.age = int(input("Enter age: "))

    def display_age(self):
        print("Age:", self.age)


# Derived class from Age (multilevel inheritance)
class ID(Age):
    def __init__(self):
        super().__init__()
        self.id = ""

    def get_id(self):
        self.id = input("Enter ID: ")

    def display_id(self):
        print("ID:", self.id)

    def display_all(self):
        self.display_name()
        self.display_age()
        self.display_id()


# Create object of the final derived class
person = ID()
person.get_name()
person.get_age()
person.get_id()

print("\n--- Person Details ---")
person.display_all()


```

### OUTPUT
![Screenshot 2025-04-28 204140](https://github.com/user-attachments/assets/c2eed383-1710-4715-af6c-3182d0d83cc9)


### RESULT
The program successfully demonstrates multilevel inheritance by collecting and displaying a person's name, age, and ID using a class hierarchy in Python.
