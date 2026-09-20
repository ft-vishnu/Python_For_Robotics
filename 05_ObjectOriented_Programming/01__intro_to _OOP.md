
# Procedure-Oriented Programming (POP)

## What is Procedure-Oriented Programming?

*Procedure-Oriented Programming (POP)* is a programming approach where the program is organized mainly around *functions or procedures*.

The main focus is on:

> *What steps or actions should the program perform?*

For example, a program may be divided into functions such as:

```python
def calculate():
    pass

def display():
    pass

def update():
    pass


Each function performs a particular task or action.

### Simple Mental Model

Think of POP as:
*Problem → Break it into steps → Create functions for those steps*


Program
   ↓
Break into tasks
   ↓
Create functions
   ↓
Execute the functions

```

### Example

Suppose we have a student program.

The program may have:

```text
Student data

name
age
marks
```

And functions:

```text
display()
calculate_marks()
update_marks()
```

The main focus is on the **functions/actions** that need to be performed.

### In One Sentence

> **Procedure-Oriented Programming is a programming approach that organizes a program mainly around functions or procedures that perform specific tasks.**

### Simple Difference from OOP

```text
POP
↓
Focus on functions / actions

OOP
↓
Focus on objects / things
```



# Object-Oriented Programming (OOP)

## What is Object-Oriented Programming?

**Object-Oriented Programming (OOP)** is a programming approach where the program is organized around **objects**.

The main focus is on:

> **What objects are there in the program, what data do they have, and what can they do?**

---

## Simple Example

Imagine we are creating a program for a **Student**.

A student has some information:

```text
Name
Age
Marks
````

A student can also perform some actions:

```text
Study
Write exam
Display details
```

In OOP, we can represent the student as an **object**.

```text
Student Object
      |
      ├── Data
      │    ├── Name
      │    ├── Age
      │    └── Marks
      │
      └── Actions
           ├── Study()
           ├── Write_exam()
           └── Display()
```

So, the student's **data and related actions are kept together**.

---

## Simple Mental Model

Think of OOP as:

**Problem → Identify objects → Give them data and actions**

```text
Program
   ↓
Identify objects
   ↓
Give objects data
   ↓
Give objects actions
   ↓
Objects work together
```

---

## Example

Suppose we create a `Student` class:

```python
class Student:

    def study(self):
        print("Student is studying")

    def write_exam(self):
        print("Student is writing exam")
```

Then we can create a student object:

```python
student1 = Student()
```

Now `student1` is an *object*.

It can perform the actions defined in the class:

```python
student1.study()
student1.write_exam()
```

---

## POP vs OOP

The basic difference is:

```text
POP
↓
Focus on functions / actions

OOP
↓
Focus on objects / things
```

### POP

We mainly think:

> "What functions do I need?"

### OOP

We mainly think:

> "What objects do I have, what data do they contain, and what can they do?"

---

## In One Sentence

> *Object-Oriented Programming is a programming approach where programs are organized around objects that contain data and related actions.*

```

**************************************************************************************************


# Object Oriented Programming (OOP)

*Object-Oriented Programming (OOP)* is a programming paradigm that revolves around the concept of *objects*, which are instances of *classes*.

The main idea behind OOP is to combine *data* and *functions that operate on the data* into a single unit called a *class*.

An *object* is a specific instance of a class, containing its own set of data and functions, which are called *methods*.

The primary goals of OOP are to improve:

- *Code organization*
- *Reusability*
- *Modularity*

This makes it easier to design, maintain, and scale complex software systems.

## Key Principles of OOP

OOP is based on several key principles:

### 1. Encapsulation

Encapsulation is the process of bundling *data (attributes)* and the *methods that operate on that data* within a single unit (class).

This helps to:

- Hide the internal workings of a class from the outside world.
- Restrict access to the internal state of an object.
- Ensure that the object's state is changed only through its methods.

### 2. Inheritance

Inheritance is a way to create a new class by deriving it from an existing class.

This allows us to *reuse and extend* the functionality of the existing class.

The new class is called the *subclass* (or derived class), and the existing class is called the *superclass* (or base class).

Inheritance enables us to create *hierarchical relationships between classes*, promoting reusability and modularity.

### 3. Polymorphism

Polymorphism refers to the ability of a function or method to take on *different forms* based on the object it is called on or the arguments it receives.

In OOP, polymorphism allows a single interface (for example, a function or method signature) to represent different types of operations on different classes or objects.

This enables us to write more *flexible and reusable code* that can work with various types of objects without knowing their specific implementation details.

### 4. Abstraction

Abstraction is the process of simplifying complex systems by breaking them down into *smaller, more manageable parts*, focusing on the essential features and hiding the complexities.

In OOP, abstraction is achieved through the use of *classes and interfaces*, which define the essential characteristics and behaviors of an object without revealing their internal implementation details.