🐍 PR-5: OOP Wrapper in Python
<p align="center"> <img src="./animation.gif" width="500"> </p> <h2 align="center">✨ Object-Oriented Programming – Wrapper ✨</h2>
📌 Introduction
This practical demonstrates the Wrapper concept in Object-Oriented Programming (OOP) using Python.

A Wrapper is used to contain an existing object and provide additional functionality without modifying the original class.

🎯 Objective
Understand the concept of Wrapper in Python.
Implement a Wrapper class using OOP.
Learn how one object can be wrapped inside another object.
Add functionality to an existing class.
💻 Program
class Student:
    def __init__(self, name, marks):
        self.name = name
        self.marks = marks


class StudentWrapper:
    def __init__(self, student):
        self.student = student

    def display(self):
        print("Student Name:", self.student.name)
        print("Marks:", self.student.marks)


student = Student("Rahul", 85)

wrapper = StudentWrapper(student)

wrapper.display()

📤 Output
Student Name: Rahul
Marks: 85

📝 Explanation
Student is the original class.
StudentWrapper is the wrapper class.
The Student object is passed to StudentWrapper.
The wrapper stores the object inside self.student.
The display() method accesses the wrapped object's data.
This demonstrates how a wrapper can add functionality to an existing object.
🧠 Wrapper Concept
        Student Object
              │
              ▼
      ┌─────────────────┐
      │ StudentWrapper  │
      └─────────────────┘
              │
              ▼
    Additional Functionality

🎬 Animation
The repository includes an animation demonstrating the Wrapper concept:

<p align="center"> <img src="./animation.gif" width="600"> </p>
Note: Upload your GIF file as animation.gif in the main repository folder.

✅ Conclusion
The Wrapper concept allows us to extend or control the behavior of an existing object without changing its original class. It is a useful OOP technique for creating flexible and reusable Python programs.

👨‍💻 Author
Raj ❤️
PR-5 | OOP Wrapper | Python 🐍
