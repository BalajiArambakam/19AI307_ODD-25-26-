# Ex.No:4(A) EXCEPTION HANDLING

## QUESTION:


## AIM:
To write a Java program to divide two integers and handle division by zero using exception handling.

## ALGORITHM :
1. Start the program
2. Import java.util.Scanner
3. Create a class named prog
4. Create the main() method
5. Declare variables num1, num2, result
6. Create a Scanner object to read input
7. Read two integers from the user
8. Use try block to perform division result = num1 / num2
9. Print the result if division is successful
10. Use catch block to handle exception
11. If division by zero occurs, print error message
12. Stop the program




## PROGRAM:
 ```
/*
Program to implement a Exception Handling using Java
Developed by: Balaji Arambakam
RegisterNumber:  212224230021
import java.util.Scanner;
class prog
{
    public static void main(String[] args)
    {
        int num1, num2, result;
        Scanner sc = new Scanner(System.in);
        num1 = sc.nextInt();
        num2 = sc.nextInt();

        try
        {
            result = num1 / num2;
            System.out.println("Result: " + result);
        }
        catch(Exception exp)
        {
            System.out.println("Error: Division by zero");
        }
    }
}
*/
```

## SOURCE CODE:







## OUTPUT:
<img width="1607" height="980" alt="image" src="https://github.com/user-attachments/assets/ac27b1a6-3ea8-4000-b869-280d834ad5d0" />



## RESULT:
Thus, the Java program to divide two integers and handle division by zero using exception handling was executed successfully.
