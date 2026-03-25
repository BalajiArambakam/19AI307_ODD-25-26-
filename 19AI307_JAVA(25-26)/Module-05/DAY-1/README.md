# Ex.No:5(A) INPUTSTREAMREADER 

## QUESTION:


## AIM:
To write a Java program to store an array of strings into a file using PrintWriter.

## ALGORITHM :
1. Start the program
2. Import java.io and java.util packages
3. Create a class named WriteArrayToFile
4. Create the main() method
5. Create a Scanner object to read input
6. Read a string from the user
7. Store the string into an array
8. Use try-with-resources to create a PrintWriter object
9. Open a file named "output.txt"
10. Use a loop to write each string into the file
11. Print success message after writing
12. Handle exceptions using catch block
13. Close the Scanner
14. Stop the program




## PROGRAM:
 ```
/*
Program to implement a InputStreamReader using Java
Developed by: Balaji Arambakam
RegisterNumber: 212224230021
import java.io.*;
import java.util.Scanner;

public class WriteArrayToFile {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String text = sc.nextLine();

        String[] data = {text};

        try (PrintWriter writer = new PrintWriter("output.txt")) {
            for (String str : data) {
                writer.println(str);
            }
            System.out.println("Array of strings written to file successfully.");
        } catch (IOException e) {
            System.out.println("An error occurred: " + e.getMessage());
        }

        sc.close();
    }
} 
*/
```

## SOURCE CODE:







## OUTPUT:
<img width="1503" height="990" alt="image" src="https://github.com/user-attachments/assets/6999e617-1811-4191-9a48-d77a7e124dbd" />



## RESULT:
Thus, the Java program to write an array of strings into a file using PrintWriter was executed successfully. 
