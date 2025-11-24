# EX3 Write a program to count the number of digits in an integer.
## DATE: 
## AIM:
To write a C program to implement Tower of Hanoi

## Algorithm
1. Start.
2. Read the number of disks n.
3. Call the recursive function tower(n, source, auxiliary, destination).
4. Recursively move disks: move n-1 disks to auxiliary, move 1 disk to destination, move n-1 disks from auxiliary to destination.
5. Stop.
## Program:
```
Program Count how many times a number appears in an array recursively.
Developed by: VAISHNAVIDEVI V
RegisterNumber:  212223040230
```
```
public class TowerOfHanoi {
    public static void tower(int n, char source, char auxiliary, char destination) {
        if (n == 1) {
            System.out.println("Move disk 1 from " + source + " to " + destination);
            return;
        }
        tower(n - 1, source, destination, auxiliary);
        System.out.println("Move disk " + n + " from " + source + " to " + destination);
        tower(n - 1, auxiliary, source, destination);
    }

    public static void main(String[] args) {

        int n = 3; 

        System.out.println("Tower of Hanoi for " + n + " disks:");
        tower(n, 'A', 'B', 'C');  // A = source, B = auxiliary, C = destination
    }
}
```

## Output:
<img width="339" height="236" alt="image" src="https://github.com/user-attachments/assets/f647ff56-7711-4329-b7b6-3ff664ef9d79" />



## Result:
Thus, the Java program to to count the number of digits in an integer is implemented successfully.
