# Ex.No:1(C) LOOPING STATEMENT

## QUESTION:


## AIM:To write a Java program to reverse a number using a while loop.


## ALGORITHM :
1. Start the program
2. Import java.util.Scanner
3. Create a class named kim
4. Create the main() method
5. Create a Scanner object to read input
6. Read an integer from the user
7. Initialize reversednum = 0
8. Repeat while num is not equal to 0
9. Find digit using digit = num % 10
10. Update reversednum using reversednum = reversednum * 10 + digit
11. Remove last digit using num = num / 10
12. Continue the loop until num becomes 0
13. Print the reversed number
14. Stop the program



## PROGRAM:
 ```
/*
Program to implement a Looping Statement using Java
Developed by: Balaji Arambakam
RegisterNumber:  212224230021

import java.util.Scanner;
public class kim
{
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);
        int num = sc.nextInt();
        int digit;
        int reversednum = 0;

        while(num != 0)
        {
            digit = num % 10;
            reversednum = reversednum * 10 + digit;
            num = num / 10;
        }

        System.out.printf("Reversed number: %d", reversednum);
        sc.close();
    }
}
*/
```

## SOURCE CODE:




## OUTPUT:
<img width="1908" height="1047" alt="image" src="https://github.com/user-attachments/assets/43f0f5ff-99b3-4fcc-b097-f7cd27dfc5ab" />




## RESULT:
Thus, the Java program to reverse a number using a while loop was executed successfully.


