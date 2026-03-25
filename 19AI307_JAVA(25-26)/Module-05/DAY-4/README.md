# Ex.No:5(D) THREAD PRIORITY

## QUESTION:


## AIM:
To write a Java program to set the name and priority of the current thread using user input.

## ALGORITHM :
1. Start the program
2. Import java.util.Scanner
3. Create a class named prog
4. Create the main() method
5. Create a Scanner object to read input
6. Read thread name from the user
7. Get current thread using Thread.currentThread()
8. Set thread name using setName()
9. Set thread priority as 2 using setPriority()
10. Print thread priority using getPriority()
11. Print thread name using getName()
12. Print thread details using currentThread object
13. Close the Scanner
14. Stop the program




## PROGRAM:
 ```
/*
Program to implement a Thread Priority Concept using Java
Developed by: Balaji Arambakam
RegisterNumber:  212224230021
import java.util.Scanner;

public class prog {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String threadName = sc.nextLine();

        Thread currentThread = Thread.currentThread();
        currentThread.setName(threadName);
        currentThread.setPriority(2);

        System.out.println("Priority of Thread: " + currentThread.getPriority());
        System.out.println("Name of Thread: " + currentThread.getName());
        System.out.println(currentThread);

        sc.close();
    }
}
*/
```

## SOURCE CODE:







## OUTPUT:
<img width="1135" height="911" alt="image" src="https://github.com/user-attachments/assets/56c93fd1-998f-48ac-8eb7-19c6e4d61012" />



## RESULT:
Thus, the Java program to set and display the name and priority of the current thread was executed successfully. 
