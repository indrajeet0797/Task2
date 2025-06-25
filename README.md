# Task2
# Student Record Management System in Java

This is a simple **console-based Student Record Management System** written in Java. It uses **Object-Oriented Programming (OOP)** concepts and an **ArrayList** to manage student records. You can perform the following operations:

- Add a student
- View all students
- Update a student
- Delete a student

---

##  Student Class

The `Student` class includes:

### Fields:
```java
private int id;
private String name;
private double marks;
```

### Constructor:
```java
public Student(int id, String name, double marks)
```

### Methods:
- `getId()`: Returns the student ID.
- `setName(String name)`: Sets the student name.
- `setMarks(double marks)`: Sets the student marks.
- `display()`: Displays the student's details.

---

## StudentManagementSystem Class

This is the main class that handles user input and provides a menu for performing various operations using an `ArrayList<Student>`.

### ➕ Add Student
```java
public static void addStudent()
```
- Prompts the user to enter ID, Name, and Marks.
- Creates a `Student` object and adds it to the `ArrayList`.

### View Students
```java
public static void viewStudents()
```
- Prints details of all students in the `ArrayList`.

### Update Student
```java
public static void updateStudent()
```
- Prompts for a student ID.
- If the student is found, asks for new name and marks, and updates them.

###  Delete Student
```java
public static void deleteStudent()
```
- Prompts for a student ID.
- Removes the student from the list if the ID matches.

---

## Main Menu Loop

The `main()` method contains a menu-driven loop:
```java
while (true) {
    System.out.println("1. Add Student");
    System.out.println("2. View Students");
    System.out.println("3. Update Student");
    System.out.println("4. Delete Student");
    System.out.println("5. Exit");
    ...
}
```
Based on the user's input, it calls the appropriate function.

---

##  How to Compile and Run

### 1. Open your terminal or command prompt.
### 2. Navigate to the folder containing the `.java` file.
### 3. Compile the Java file:
```bash
javac StudentManagementSystem.java
```

### 4. Run the compiled class:
```bash
java StudentManagementSystem
```

---

## Sample Output

```
--- Student Record Management ---
1. Add Student
2. View Students
3. Update Student
4. Delete Student
5. Exit
Choose an option: 1
Enter ID: 101
Enter Name: Alice
Enter Marks: 89.5
Student added successfully.
```

---

## Concepts Used

- Java Class and Object
- Encapsulation (private fields + public methods)
- Java Collections (`ArrayList`)
- Loops and Conditionals
- Scanner for user input

---

##  File Structure

```
StudentRecordSystem/
│
├── StudentManagementSystem.java
└── README.md
```

---

## Summary

This basic Java application is ideal for beginners learning how to:
- Work with user input
- Apply OOP in Java
- Handle lists with `ArrayList`
- Build a CRUD system via a menu-based console application

It can also be extended to GUI-based systems or database integration in the future.
