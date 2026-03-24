# Ex.No:4(C)  COMPOSITION IN JAVA

## QUESTION:


## AIM:
To write a Java program to demonstrate composition by creating a Library class that contains multiple Book objects and displays their details.

## ALGORITHM :
1. Start the program
2. Import java.util package
3. Create a class named Book
4. Declare variables title and author
5. Create a constructor to initialize title and author
6. Create a method getDetails() to return book details
7. Create a class named Library
8. Declare a List to store Book objects
9. Initialize the list using ArrayList
10. Create a method addBook(title, author)
11. Create a new Book object and add it to the list
12. Create a method showBooks()
13. If list is empty print "No books in the library"
14. Otherwise print all book details using loop
15. Create a class named CompositionExample
16. Create the main() method
17. Create Scanner object to read input
18. Read number of books n
19. Use loop to read title and author for each book
20. Call addBook() to store books
21. Call showBooks() to display all books
22. Stop the program




## PROGRAM:
 ```
/*
Program to implement a Composition Concepts in Java
Developed by: Balaji Arambakam
RegisterNumber:  212224230021
import java.util.*;

public class CompositionExample {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        Library library = new Library();

        int n = sc.nextInt();
        sc.nextLine();

        for (int i = 0; i < n; i++) {
            String title = sc.nextLine();
            String author = sc.nextLine();
            library.addBook(title, author);
        }

        library.showBooks();
        sc.close();
    }
}

class Book {
    private String title;
    private String author;

    public Book(String title, String author) {
        this.title = title;
        this.author = author;
    }

    public String getDetails() {
        return title + " by " + author;
    }
}

class Library {
    private List<Book> books = new ArrayList<>();

    public void addBook(String title, String author) {
        books.add(new Book(title, author));
    }

    public void showBooks() {
        if (books.isEmpty()) {
            System.out.println("No books in the library.");
        } else {
            System.out.println("Books in Library:");
            for (Book b : books) {
                System.out.println("- " + b.getDetails());
            }
        }
    }
}
*/
```

## SOURCE CODE:


## OUTPUT:
<img width="1415" height="743" alt="image" src="https://github.com/user-attachments/assets/642b34f4-86fd-46d2-906e-7cde15d010d1" />



## RESULT:
Thus, the Java program to demonstrate composition using Library and Book classes was executed successfully
