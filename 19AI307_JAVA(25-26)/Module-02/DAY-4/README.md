# Ex.No:2(D) VARIABLE SCOPE AND CONSTRUCTOR

## QUESTION:


## AIM:To write a Java program to access a static variable using both the class name and an object.


## ALGORITHM :
1. Start the program
2. Import java.util package
3. Create a class named prog
4. Declare a static integer variable n
5. Create the main() method
6. Create a Scanner object to read input
7. Read an integer from the user
8. Create an object of class prog
9. Assign the input value to the static variable using the object
10. Display the value using the class name (prog.n)
11. Display the value using the object (p.n)
12. Stop the program




## PROGRAM:
 ```
/*
Program to implement a Variable scope and Constructor using Java
Developed by: Balaji Arambakam
RegisterNumber: 212224230021

 import java.util.*;
class prog
{
    static int n;
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);
        int num = sc.nextInt();
        prog p = new prog();
        p.n = num;
        System.out.println("Accessing using class name: " + prog.n);
        System.out.println("Accessing using object: " + p.n);
    }
}
*/
```

## SOURCE CODE:







## OUTPUT:
<img width="1913" height="1048" alt="image" src="https://github.com/user-attachments/assets/1c8878de-1266-40c4-8624-e66410e80388" />




## RESULT:
Thus, the Java program to access a static variable using both class name and object was executed successfully.

