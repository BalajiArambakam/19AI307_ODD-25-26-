# Ex.No:1(D) ARRAYS

## QUESTION:


## AIM:
To write a Java program to count the number of even and odd elements in an array.


## ALGORITHM :

1. Start the program
2. Import java.util.Scanner
3. Create a class named evenodd
4. Create the main() method
5. Create a Scanner object to read input
6. Read the size of the array
7. Create an integer array of given size
8. Initialize two counters counte = 0 and counto = 0
9. Use a for loop from i = 0 to size - 1
10. Read each array element
11. If the element is divisible by 2 then increase counte
12. Otherwise increase counto
13. After the loop print number of even elements
14. Print number of odd elements
15. Stop the program



## PROGRAM:
 ```
/*
Program to implement a Array concept using Java
Developed by: Balaji Arambakam
RegisterNumber:  2122242300021

import java.util.Scanner;
public class evenodd
{
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);
        int size = sc.nextInt();
        int arr[] = new int[size];
        int counte = 0;
        int counto = 0;

        for(int i = 0; i < size; i++)
        {
            arr[i] = sc.nextInt();
            if(arr[i] % 2 == 0)
            {
                counte++;
            }
            else
            {
                counto++;
            }
        }

        System.out.printf("Number of even elements: %d\n", counte);
        System.out.printf("Number of odd elements: %d\n", counto);
    }
}
*/
```

## SOURCE CODE:







## OUTPUT:
<img width="1905" height="1050" alt="image" src="https://github.com/user-attachments/assets/ac045692-11d8-4f18-82ad-7ebe87aa91b8" />




## RESULT:
Thus, the Java program to count the number of even and odd elements in an array was executed successfully.

