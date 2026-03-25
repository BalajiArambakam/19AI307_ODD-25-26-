# Ex.No:5(B) SERIALIZATION AND DESERIALIZATION 

## QUESTION:


## AIM:
To write a Java program to demonstrate writing and reading UTF strings using DataOutputStream and DataInputStream.

## ALGORITHM :
1. Start the program
2. Import java.io and java.util packages
3. Create a class named DataInputStreamUTFExample
4. Create the main() method
5. Create a Scanner object to read input
6. Read a string from the user
7. Create FileOutputStream for a file
8. Wrap it with DataOutputStream
9. Write the string using writeUTF()
10. Close the output stream
11. Create FileInputStream for the same file
12. Wrap it with DataInputStream
13. Read the string using readUTF()
14. Store the result in a variable
15. Display the read string
16. Close the input stream
17. Handle exceptions using try-catch
18. Stop the program




## PROGRAM:
 ```
/*
Program to implement a Serialization and Deserialization using Java
Developed by: Balaji Arambakam
RegisterNumber:  212224230021
import java.io.*;
import java.util.Scanner;

public class DataInputStreamUTFExample {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        try {
            String input = sc.nextLine();

            FileOutputStream fos = new FileOutputStream("utfdata.dat");
            DataOutputStream dos = new DataOutputStream(fos);
            dos.writeUTF(input);
            dos.close();

            FileInputStream fis = new FileInputStream("utfdata.dat");
            DataInputStream dis = new DataInputStream(fis);
            String result = dis.readUTF();
            dis.close();

            System.out.println("String read from file: " + result);

        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}
*/
```

## SOURCE CODE:







## OUTPUT:
<img width="1237" height="1000" alt="image" src="https://github.com/user-attachments/assets/b9456ddd-5247-41ed-9a94-845097d14a5c" />



## RESULT:
Thus, the Java program to write and read UTF strings using DataInputStream and DataOutputStream was executed successfully
