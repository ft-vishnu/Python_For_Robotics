
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

## Object-Oriented Programming (OOP)

*Object-Oriented Programming (OOP)* is a way of writing programs by organizing them around *objects*.

An object represents a *thing* in the program.

For example:

- Student
- Car
- Robot
- Drone
- Bank Account

Each object can have:

- *Data* → information about the object
- *Methods* → actions that the object can perform

### Simple Example

Think about a *Car*.

A car has data:

- Brand
- Color
- Speed

A car can perform actions:

- Start
- Stop
- Accelerate
- Brake

So we can think of it as:

```text
Car
│
├── Data
│   ├── Brand
│   ├── Color
│   └── Speed
│
└── Actions
    ├── Start()
    ├── Stop()
    ├── Accelerate()
    └── Brake()
```

This is the basic idea of OOP:

> *Keep the data and the actions related to that data together.*

---

## Why Do We Use OOP?

As programs become larger, managing everything as separate variables and functions can become difficult.

OOP helps us organize a large program into smaller, meaningful objects.

The main goals are:

- *Better organization* → Keep related things together.
- *Reusability* → Reuse existing code instead of writing it again.
- *Modularity* → Divide a large program into smaller, manageable parts.
- *Maintainability* → Make the program easier to understand and modify.

---

# Key Principles of OOP

There are four important concepts commonly associated with OOP:

1. Encapsulation
2. Inheritance
3. Polymorphism
4. Abstraction

These concepts help us organize and manage objects in different ways.

---

## 1. Encapsulation

### Basic Idea

*Encapsulation* means keeping the *data* and the *methods that work with that data* together inside an object/class.

Think of a capsule.

The important things are kept together inside it.

```text
Object
│
├── Data
│
└── Methods
```

For example, a bank account has:

```text
Bank Account
│
├── Data
│   └── Balance
│
└── Methods
    ├── Deposit()
    └── Withdraw()
```

The methods are responsible for working with the account's data.

### Simple Idea

> *Encapsulation = Keep related data and methods together.*

---

## 2. Inheritance

### Basic Idea

*Inheritance* means creating a new class using an existing class.

The new class can *reuse* things from the existing class and can also add its own features.

For example:

```text
Animal
│
├── Dog
└── Cat
```

A general `Animal` class may have:

```text
Animal
├── eat()
└── sleep()
```

A `Dog` can inherit these features and also have:

```text
Dog
├── eat()
├── sleep()
└── bark()
```

The `Dog` does not need to create `eat()` and `sleep()` from scratch.

### Simple Idea

> *Inheritance = Create a new class by reusing features from an existing class.*

---

## 3. Polymorphism

### Basic Idea

*Polymorphism* means that the *same method or operation can behave differently depending on the object*.

For example, different animals can have a method called `sound()`.

```text
Dog → sound() → Bark

Cat → sound() → Meow

Cow → sound() → Moo
```

The method has the same general purpose:

```text
sound()
```

But each object can perform it differently.

### Simple Idea

> *Polymorphism = Same operation, different behavior.*

---

## 4. Abstraction

### Basic Idea

*Abstraction* means showing only the *important information* and hiding unnecessary internal details.

Think about driving a car.

You use:

```text
Steering wheel
Brake
Accelerator
Gear
```

You do not need to know exactly how the engine internally works every time you drive.

You only interact with the important controls.

Similarly, in programming, we can use an object through its important features without needing to know all of its internal implementation.

### Simple Idea

> *Abstraction = Show what is necessary and hide unnecessary complexity.*

---

# Simple Summary

```text
OOP
│
├── Objects
│   ├── Data
│   └── Methods
│
└── Four Important Concepts
    │
    ├── Encapsulation
    │   └── Keep data and methods together
    │
    ├── Inheritance
    │   └── Reuse features from another class
    │
    ├── Polymorphism
    │   └── Same operation, different behavior
    │
    └── Abstraction
        └── Show important things, hide complexity
```

## One-Line Mental Model

> *OOP is a way of organizing a program around objects, where objects contain data and actions, and concepts like encapsulation, inheritance, polymorphism, and abstraction help us manage those objects.*