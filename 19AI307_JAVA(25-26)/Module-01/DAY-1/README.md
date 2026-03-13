# Ex.No:1(A) INTRODUCTION TO JAVA PROGRAMMING, DATA TYPES, VARIABLES AND OPERATORS

## QUESTION:


## AIM:To write a Java program that reads a name from the user and prints a greeting message using that name.


## ALGORITHM :
Start the program.

Import the Scanner class from java.util package.

Create a class named Main.

Inside the main method, create a Scanner object to read input from the user.

Read the name entered by the user using nextLine().

Store the input in a String variable.

Display the message "Hello, [name]" using System.out.println().

End the program.



## PROGRAM:
 ```
import java.util.Scanner;
public class Main
{
    public static void main(String[] args)
    {
        Scanner sci = new Scanner(System.in);
        String man = sci.nextLine();
        System.out.println("Hello, " + man);
    }
}
```

## Sourcecode.java:







## OUTPUT:
<img width="1903" height="1052" alt="image" src="https://github.com/user-attachments/assets/1b1fbf88-5348-4217-abc0-4afc13bcd9fe" />





## RESULT:
Thus, the Java program to read a name from the user and display a greeting message was successfully executed.
