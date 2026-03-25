# Ex.No:5(C)  FILE HANDLING USING JAVA
## QUESTION:


## AIM:
To write a Java program to count the number of words present in a file.

## ALGORITHM :
1. Start the program
2. Import java.io and java.util packages
3. Create a class named CountWordsInFile
4. Create the main() method
5. Create a Scanner object to read input
6. Read a line of text from the user
7. Create a file using FileWriter
8. Write the input text into the file
9. Close the FileWriter
10. Initialize wordCount = 0
11. Open the file using FileReader
12. Use Scanner to read the file content
13. While there are words in the file
14. Read each word and increment wordCount
15. Close file and scanner
16. Display the word count
17. Handle exceptions using try-catch
18. Stop the program





## PROGRAM:
 ```
/*
Program to implement a File Handling using Java
Developed by: Balaji Arambakam
RegisterNumber:  212224230021
import java.io.FileWriter;
import java.io.FileReader;
import java.io.IOException;
import java.util.Scanner;

public class CountWordsInFile {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        String fileName = "userwords.txt";

        String input = scanner.nextLine();

        try {
            FileWriter writer = new FileWriter(fileName);
            writer.write(input);
            writer.close();
        } catch (IOException e) {
            System.out.println("Error writing to the file.");
            e.printStackTrace();
            scanner.close();
            return;
        }

        int wordCount = 0;
        try {
            FileReader reader = new FileReader(fileName);
            Scanner fileScanner = new Scanner(reader);

            while (fileScanner.hasNext()) {
                fileScanner.next();
                wordCount++;
            }

            fileScanner.close();
            reader.close();
        } catch (IOException e) {
            System.out.println("Error reading the file.");
            e.printStackTrace();
        }

        System.out.println("Number of words in the file: " + wordCount);
        scanner.close();
    }
}
*/
```

## SOURCE CODE:







## OUTPUT:
<img width="1424" height="431" alt="image" src="https://github.com/user-attachments/assets/8b87f851-9c99-46dc-8e17-b12226a1f196" />



## RESULT:
Thus, the Java program to count the number of words in a file was executed successfully.
