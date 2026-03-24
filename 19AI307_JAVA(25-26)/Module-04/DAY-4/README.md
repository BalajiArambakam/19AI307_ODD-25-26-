# Ex.No:4(D) DESIGN PATTERN -- ABSTRACT FACTORY

## QUESTION:


## AIM:
To write a Java program to simulate a fan speed controller using the State Design Pattern, where speed changes as Off → Low → Medium → High → Off.

## ALGORITHM :
1. Start the program
2. Import java.util.Scanner
3. Create an interface FanState with methods next() and show()
4. Create a class Fan with a variable of type FanState
5. Initialize the fan state as OffState
6. Create method setState() to change state
7. Create method next() to move to next state
8. Create method showState() to display current state
9. Create class OffState implementing FanState
10. In next(), change state to LowState
11. In show(), print "Fan is Off"
12. Create class LowState implementing FanState
13. In next(), change state to MediumState
14. In show(), print "Fan is on Low"
15. Create class MediumState implementing FanState
16. In next(), change state to HighState
17. In show(), print "Fan is on Medium"
18. Create class HighState implementing FanState
19. In next(), change state to OffState
20. In show(), print "Fan is on High"
21. Create class prog with main() method
22. Create Scanner object and Fan object
23. Read user input in loop
24. If input is "next", change state and display it
25. If input is "exit", stop the loop
26. Stop the program



## PROGRAM:
 ```
/*
Program to implement a Abstract Factory Pattern using Java
Developed by: Balaji Arambakam
RegisterNumber:  212224230021
import java.util.Scanner;

interface FanState {
    void next(Fan fan);
    void show();
}

class Fan {
    private FanState state;

    public Fan() {
        state = new OffState();
    }

    public void setState(FanState state) {
        this.state = state;
    }

    public void next() {
        state.next(this);
    }

    public void showState() {
        state.show();
    }
}

class OffState implements FanState {
    public void next(Fan fan) {
        fan.setState(new LowState());
    }

    public void show() {
        System.out.println("Fan is Off");
    }
}

class LowState implements FanState {
    public void next(Fan fan) {
        fan.setState(new MediumState());
    }

    public void show() {
        System.out.println("Fan is on Low");
    }
}

class MediumState implements FanState {
    public void next(Fan fan) {
        fan.setState(new HighState());
    }

    public void show() {
        System.out.println("Fan is on Medium");
    }
}

class HighState implements FanState {
    public void next(Fan fan) {
        fan.setState(new OffState());
    }

    public void show() {
        System.out.println("Fan is on High");
    }
}

class prog {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        Fan fan = new Fan();

        while (true) {
            String input = sc.nextLine();

            if (input.equals("next")) {
                fan.next();
                fan.showState();
            } else if (input.equals("exit")) {
                break;
            }
        }

        sc.close();
    }
}
*/
```

## SOURCE CODE:







## OUTPUT:
<img width="851" height="547" alt="image" src="https://github.com/user-attachments/assets/27735b91-bfd4-4f9b-a783-569a3a4dbed6" />



## RESULT:
Thus, the Java program to simulate a fan speed controller using the State Design Pattern was executed successfully.
