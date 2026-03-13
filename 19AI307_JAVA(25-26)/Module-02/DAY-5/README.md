# Ex.No:2(E) ACCESS MODIFIERS

## QUESTION:


## AIM:
To write a Java program to demonstrate that a final method cannot be overridden in a subclass.

## ALGORITHM :
1. Start the program
2. Create a class named SpeedLimit
3. Create a final method displayLimit()
4. Inside the method print "Max Speed: 80 km/h"
5. Create a subclass named HighwaySpeed that extends SpeedLimit
6. Do not override the final method in the subclass
7. Create another class named prog
8. Create the main() method
9. Create an object of HighwaySpeed
10. Call the displayLimit() method using the object
11. Display the output
12. Stop the program



## PROGRAM:
 ```
/*
Program to implement a Access Modifiers using Java
Developed by: Balaji Arambakam
RegisterNumber:  212224230021

class SpeedLimit {
    final void displayLimit() {
        System.out.println("Max Speed: 80 km/h");
    }
}

class HighwaySpeed extends SpeedLimit {
}

class prog {
    public static void main(String[] args)
    {
        HighwaySpeed hs = new HighwaySpeed();
        hs.displayLimit();
    }
}
*/
```

## SOURCE CODE:







## OUTPUT:
<img width="1919" height="1053" alt="image" src="https://github.com/user-attachments/assets/317fa48f-8afe-4751-be0d-ce1205ca0e38" />



## RESULT:
Thus, the Java program to demonstrate that a final method cannot be overridden in a subclass was executed successfully. 

