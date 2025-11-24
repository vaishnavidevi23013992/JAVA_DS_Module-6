# EX 1 You’re creating a health monitoring device which stores several sensor readings in an array. To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.
## DATE:
## AIM:
To write a JAVA program To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.

## Algorithm
1. Start
2. Read n – the number of heartbeat values.
3. Read the n heartbeat values into an array.
4. Call the recursive method findMin(arr, index)
5. Recursive logic:
6. Display the minimum heartbeat value returned by the recursive function.
7. Stop

## Program:
```
Program Count how many times a number appears in an array recursively.
Developed by: VAISHNAVIDEVI V
RegisterNumber:  212223040230
```
```
import java.util.Scanner;

public class MinValueRecursion {
    public static int findMin(int[] arr, int index) {
        if (index == arr.length - 1) {
            return arr[index];
        }
        int minOfRest = findMin(arr, index + 1);
        return Math.min(arr[index], minOfRest);
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter number of heartbeat readings: ");
        int n = sc.nextInt();
        int[] heartbeat = new int[n];
        System.out.println("Enter the heartbeat values:");
        for (int i = 0; i < n; i++) {
            heartbeat[i] = sc.nextInt();
        }
        int minValue = findMin(heartbeat, 0);
        System.out.println("Minimum (Lowest) Heartbeat Value = " + minValue);
    }
}

```

## Output:
<img width="459" height="235" alt="image" src="https://github.com/user-attachments/assets/d857b94f-a6ea-4ccc-a2fd-58ac74075c41" />



## Result:
Thus the JAVA prograM ti find the minimum value (e.g., lowest heartbeat), implement a recursive method has implemented successfully
