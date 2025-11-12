# Ex2 Count how many times a number appears in an array recursively.

## DATE:
11.11.2025  

## AIM:
To write a Java program to count how many times a number appears in an array recursively.

## Algorithm
1. Start the program.  
2. Read the number of elements and store them in an array.  
3. Get the number to be counted from the user.  
4. Define a recursive function `countOccurrences()` that returns how many times the number appears.  
5. Use base and recursive conditions to count occurrences.  
6. Display the result.  
7. Stop the program.  

## Program:
```java
/*
Program to count how many times a number appears in an array recursively.
Developed by: Selshiya F
RegisterNumber: 212224060241
*/
import java.util.Scanner;

public class CountOccurrencesRecursive {
    static int countOccurrences(int arr[], int n, int key) {
        if (n == 0)
            return 0;
        return (arr[n - 1] == key ? 1 : 0) + countOccurrences(arr, n - 1, key);
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter number of elements: ");
        int n = sc.nextInt();
        int arr[] = new int[n];
        System.out.println("Enter the elements:");
        for (int i = 0; i < n; i++)
            arr[i] = sc.nextInt();
        System.out.print("Enter number to count: ");
        int key = sc.nextInt();
        System.out.println("The number " + key + " appears " + countOccurrences(arr, n, key) + " times.");
        sc.close();
    }
}
```
## OUTPUT 
<img width="946" height="187" alt="image" src="https://github.com/user-attachments/assets/e41c957e-3086-42ac-bb24-f59e0d5f2411" />
## RESULT
Thus, the Java program to count how many times a number appears in an array recursively is implemented successfully.
