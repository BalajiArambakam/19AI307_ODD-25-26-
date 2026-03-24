# Ex.No:4(D) DESIGN PATTERN  ---- BEHAVIOUR PATTERN

## QUESTION:


## AIM:
To write a Java program to implement the MVC (Model View Controller) pattern for managing a bank account with deposit and withdrawal operations.

## ALGORITHM :
1. Start the program
2. Import java.util package
3. Create class Account (Model)
4. Declare variable balance
5. Create constructor to initialize balance
6. Create method getBalance()
7. Create method deposit(amount) to add money
8. Create method withdraw(amount)
9. If amount > balance return false
10. Else deduct amount and return true
11. Create class AccountView (View)
12. Create method showBalance() to display balance
13. Create method showFail() for insufficient balance
14. Create class AccountController (Controller)
15. Store Account and AccountView objects
16. Create deposit() method to update model and view
17. Create withdraw() method to check and update view
18. Create class Main
19. Create main() method
20. Read initial balance and number of operations
21. Create model, view, and controller objects
22. Loop through operations
23. If operation is deposit call controller.deposit()
24. Else call controller.withdraw()
25. Display results
26. Stop the program




## PROGRAM:
 ```
/*
Program to implement a Behaviour Pattern using Java
Developed by: Balaji Arambakam
RegisterNumber:  212224230021
import java.util.*;

class Account {
    private double balance;

    public Account(double balance) {
        this.balance = balance;
    }

    public double getBalance() { return balance; }

    public void deposit(double amount) {
        balance += amount;
    }

    public boolean withdraw(double amount) {
        if (amount > balance) return false;
        balance -= amount;
        return true;
    }
}

class AccountView {
    public void showBalance(double balance) {
        System.out.printf("Current Balance: ₹%.2f%n", balance);
    }

    public void showFail() {
        System.out.println("Withdrawal failed: insufficient balance.");
    }
}

class AccountController {
    private Account model;
    private AccountView view;

    public AccountController(Account model, AccountView view) {
        this.model = model;
        this.view = view;
    }

    public void deposit(double amt) {
        model.deposit(amt);
        view.showBalance(model.getBalance());
    }

    public void withdraw(double amt) {
        if (model.withdraw(amt))
            view.showBalance(model.getBalance());
        else
            view.showFail();
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        double initial = Double.parseDouble(sc.nextLine());
        int n = Integer.parseInt(sc.nextLine());

        Account model = new Account(initial);
        AccountView view = new AccountView();
        AccountController controller = new AccountController(model, view);

        for (int i = 0; i < n; i++) {
            String[] parts = sc.nextLine().split(" ");
            String op = parts[0];
            double amt = Double.parseDouble(parts[1]);

            if (op.equals("deposit"))
                controller.deposit(amt);
            else
                controller.withdraw(amt);
        }
    }
}
*/
```

## SOURCE CODE:







## OUTPUT:
<img width="1135" height="790" alt="image" src="https://github.com/user-attachments/assets/5b40dadb-8a26-4429-adb1-d2fc60aa4c42" />



## RESULT:
Thus, the Java program to implement the MVC pattern for managing a bank account with deposit and withdrawal operations was executed successfully.
