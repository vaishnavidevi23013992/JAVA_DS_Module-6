# Ex2 Count how many times a number appears in an array recursively.
## DATE: 
## AIM:
To write a Java program to Count how many times a number appears in an array recursively.

## Algorithm
1. Start
2. Read the array and the number to be counted.
3. Call the recursive function with starting index.
4. Recursively count occurrences until the end of the array.
5. Display the count and stop.
## Program:
```
Program Count how many times a number appears in an array recursively.
Developed by: VAISHNAVIDEVI V
RegisterNumber:  212223040230
```
```
import java.util.Scanner;
public class CountOccurrencesRecursion {
    public static int count(int[] arr, int index, int x) {
        if (index == arr.length) {
            return 0;
        }
        if (arr[index] == x) {
            return 1 + count(arr, index + 1, x);
        }
        return count(arr, index + 1, x);
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter number of elements: ");
        int n = sc.nextInt();

        int[] arr = new int[n];
        System.out.println("Enter array elements:");
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }
        System.out.print("Enter number to count: ");
        int x = sc.nextInt();
        int result = count(arr, 0, x);
        System.out.println("The number " + x + " appears " + result + " times.");
    }
}

```

## Output:
<img width="342" height="336" alt="image" src="https://github.com/user-attachments/assets/307ba6d9-5022-45b1-a502-94f23bd3aefa" />



## Result:
Thus, the Java program to Count how many times a number appears in an array recursively is implemented successfully.
