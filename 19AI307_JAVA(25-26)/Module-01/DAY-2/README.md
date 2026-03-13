# Ex.No:1(B) CONDITIONAL STATEMENT

## QUESTION:


## AIM:To write a Java program to analyze a 3-digit number and determine the maze behavior based on its digits.


## ALGORITHM :
1. Start the program
2. Import java.util.Scanner
3. Create a class named halwa
4. Create the main() method
5. Create a Scanner object to read input
6. Read a three digit integer from the user
7. Find first digit using first = num / 100
8. Find middle digit using mid = (num / 10) % 10
9. Find last digit using last = num % 10
10. Calculate total = first + mid + last
11. If mid == 0 print "Freezes"
12. Else if total == 15 print "Reflects"
13. Else if first is odd and last is even print "Opens"
14. Else print "Collapses"
15. Stop the program




## PROGRAM:
 ```
/*
Program to implement a conditional statement using Java
Developed by: Balaji Arambakam
RegisterNumber:  212224230021

import java.util.Scanner;
public class halwa
{
    public static void main(String[] args)
    {
        Scanner p = new Scanner(System.in);
        int num = p.nextInt();
        int first = num/100;
        int mid = (num/10)%10;
        int last = num%10;
        int total = first + mid + last;

        if(mid == 0)
        {
            System.out.print("Freezes");
        }
        else if(total == 15)
        {
            System.out.print("Reflects");
        }
        else if(first%2 == 1 && last%2 == 0)
        {
            System.out.print("Opens");
        }
        else
        {
            System.out.print("Collapses");
        }
    }
}
*/
```

## SOURCE CODE:







## OUTPUT:

<img width="1913" height="1048" alt="image" src="https://github.com/user-attachments/assets/8039452e-97b8-41d4-bce3-5ec1e27a9d29" />




## RESULT:
Thus, the Java program to determine the maze behavior based on the digits of a three digit access code was executed successfully.

