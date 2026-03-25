# Ex.No:5(E) MULTITHREADING -SYNCHRONIZATION

## QUESTION:


## AIM:
To write a Java program to calculate squares of numbers using multithreading with ExecutorService.

## ALGORITHM :
1. Start the program
2. Import java.util and java.util.concurrent packages
3. Create a class named Main
4. Create the main() method
5. Create a Scanner object to read input
6. Read integer n (number of inputs)
7. Create a fixed thread pool with 2 threads
8. Create a list to store Future results
9. Use a loop from 0 to n-1
10. Read each integer value
11. Submit a task to thread pool to compute square
12. Store Future result in list
13. Iterate through Future list
14. Get result using f.get()
15. Print each square result
16. Shutdown the thread pool
17. Stop the program



## PROGRAM:
 ```
/*
Program to implement a Synchronization concept using Java
Developed by: Balaji Arambakam
RegisterNumber:  212224230021
import java.util.*;
import java.util.concurrent.*;

public class Main {
    public static void main(String[] args) throws Exception {
        Scanner sc = new Scanner(System.in);
        int n = Integer.parseInt(sc.nextLine());

        ExecutorService pool = Executors.newFixedThreadPool(2);
        List<Future<String>> results = new ArrayList<>();

        for (int i = 0; i < n; i++) {
            int val = Integer.parseInt(sc.nextLine());
            results.add(pool.submit(() -> "Square: " + (val * val)));
        }

        for (Future<String> f : results) {
            System.out.println(f.get());
        }

        pool.shutdown();
    }
}
*/
```

## SOURCE CODE:







## OUTPUT:
<img width="727" height="548" alt="Screenshot 2026-03-25 140022" src="https://github.com/user-attachments/assets/4c69a14a-77d4-4910-953a-613934a77846" />



## RESULT:
Thus, the Java program to compute squares of numbers using ExecutorService and multithreading was executed successfully. 
