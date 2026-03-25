# Ex.No:4(B)  IMPLEMENT SOLID PRINCIPLES IN JAVA PROGRAM 

## QUESTION:


## AIM:
To write a Java program to implement the Singleton design pattern and track the number of times the Master Power Switch is accessed.

## ALGORITHM :
1. Start the program
2. Import java.util package
3. Create a class named MasterPowerSwitch
4. Declare a private static object instance
5. Declare a private variable accessCount initialized to 0
6. Create a private constructor to restrict object creation
7. Create a public static method getInstance()
8. If instance is null, create a new object
9. Return the same instance every time
10. Create a method logAccess()
11. Increment accessCount and return it
12. Create a class named prog
13. Create the main() method
14. Create a Scanner object to read input
15. Read number of users n
16. Use a loop from 0 to n-1
17. Read player name
18. Call getInstance() to get the same object
19. Call logAccess() to update count
20. Print player name with access count
21. Stop the program





## PROGRAM:
 ```
/*
Program to implement a SOLID Principles in Java Program
Developed by: Balaji Arambakam
RegisterNumber:  212224230021
import java.util.*;

class MasterPowerSwitch 
{
    private static MasterPowerSwitch instance = null;
    private int accessCount = 0;

    private MasterPowerSwitch() {}

    public static MasterPowerSwitch getInstance()
    {
        if (instance == null)
        {
            instance = new MasterPowerSwitch();
        }
        return instance;
    }

    public int logAccess()
    {
        accessCount++;
        return accessCount;
    }
}

public class prog 
{
    public static void main(String[] args) 
    {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        sc.nextLine();

        for (int i = 0; i < n; i++) 
        {
            String player = sc.nextLine();
            MasterPowerSwitch power = MasterPowerSwitch.getInstance();
            int count = power.logAccess();
            System.out.println(player + " accessed Master Power Switch. Total accesses so far: " + count);
        }
    }
}
*/
```

## SOURCE CODE:




## OUTPUT:
<img width="1495" height="458" alt="image" src="https://github.com/user-attachments/assets/cc5a7787-b2aa-4f22-8200-ddafe66b6e03" />



## RESULT:
Thus, the Java program to implement the Singleton design pattern and track access count using a single object instance was executed successfully. 
