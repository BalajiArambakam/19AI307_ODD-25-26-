# Ex.No:2(A) CLASS AND OBJECT

## QUESTION:


## AIM:To write a Java program to create a class Mobile with attributes brand, storage, and color and display the details of two mobiles.


## ALGORITHM :
1. Start the program
2. Import java.util.Scanner
3. Create a class named Mobile
4. Declare attributes brand, storage, and color
5. Create a method mod() to display mobile details
6. Create another class named Main
7. Create the main() method
8. Create a Scanner object to read input
9. Create the first Mobile object
10. Read brand, storage, and color for the first mobile
11. Store the values in the object's attributes
12. Create the second Mobile object
13. Read brand, storage, and color for the second mobile
14. Store the values in the object's attributes
15. Call the mod() method to print the details of both mobiles
16. Stop the program



## PROGRAM:
 ```
/*
Program to implement a Class and Objects using Java
Developed by: Balaji Arambakam
RegisterNumber: 212224230021

 import java.util.Scanner;
class Mobile
{
    String brand;
    int storage;
    String color;

    void mod()
    {
        System.out.println(brand + " | " + storage + "GB" + " | " + color);
    }
}

public class Main
{
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);

        Mobile phone1 = new Mobile();
        phone1.brand = sc.next();
        phone1.storage = sc.nextInt();
        phone1.color = sc.next();

        Mobile phone = new Mobile();
        phone.brand = sc.next();
        phone.storage = sc.nextInt();
        phone.color = sc.next();

        phone1.mod();
        phone.mod();
    }
}
*/
```

## SOURCE CODE:







## OUTPUT:

<img width="1904" height="1066" alt="image" src="https://github.com/user-attachments/assets/3207a0a7-6136-4369-867a-67e3c5d61a00" />



## RESULT:
Thus, the Java program to create a Mobile class and display the details of two mobiles was executed successfully. 

