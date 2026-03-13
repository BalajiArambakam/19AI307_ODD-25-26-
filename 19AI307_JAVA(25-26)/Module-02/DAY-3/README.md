# Ex.No:2(C) ACCESS SPECIFIERS

## QUESTION:


## AIM:
To write a Java program to create a Student class with private variables student_id, student_name, and grade, and use getter and setter methods with validation to add a grade.

## ALGORITHM :
1. Start the program
2. Import java.util.Scanner
3. Create a class named Student
4. Declare private variables student_id, student_name, and grade
5. Create setter methods setStudentId() and setStudentName()
6. Create getter methods getStudentId(), getStudentName(), and getGrade()
7. Create a method addGrade(int grade)
8. Check if the grade is between 0 and 100
9. If valid, store the grade and return true
10. Otherwise return false
11. Create a display() method to print student details
12. Create another class named Main
13. Create the main() method
14. Create a Scanner object to read input
15. Create a Student object
16. Read student id, student name, and grade from the user
17. Set id and name using setter methods
18. Call addGrade() method to validate and store grade
19. If valid, call display() method
20. Otherwise print invalid grade message
21. Stop the program





## PROGRAM:
 ```
/*
Program to implement a Access Specifiers using Java
Developed by: Balaji Arambakam 
RegisterNumber:  212224230021

import java.util.Scanner;

class Student {
    private int student_id;
    private String student_name;
    private int grade;

    public void setStudentId(int student_id) {
        this.student_id = student_id;
    }

    public void setStudentName(String student_name) {
        this.student_name = student_name;
    }

    public int getStudentId() {
        return student_id;
    }

    public String getStudentName() {
        return student_name;
    }

    public int getGrade() {
        return grade;
    }

    public boolean addGrade(int grade) {
        if (grade >= 0 && grade <= 100) {
            this.grade = grade;
            return true;
        } else {
            return false;
        }
    }

    public void display() {
        System.out.println("Student ID: " + student_id);
        System.out.println("Student Name: " + student_name);
        System.out.println("Grade: " + grade);
        System.out.println("-----------------------");
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        Student s = new Student();

        int id = sc.nextInt();
        sc.nextLine();
        String name = sc.nextLine();
        int grade = sc.nextInt();

        s.setStudentId(id);
        s.setStudentName(name);

        if (s.addGrade(grade)) {
            s.display();
        } else {
            System.out.println("Invalid grade. Please enter a value between 0 and 100.");
        }
    }
}
*/
```

## SOURCE CODE:







## OUTPUT:

<img width="1914" height="1097" alt="image" src="https://github.com/user-attachments/assets/9b5bdd83-d15c-4531-8920-cdf679e49a10" />


## RESULT:
Thus, the Java program to create a Student class using encapsulation with getter and setter methods and grade validation was executed successfully.

