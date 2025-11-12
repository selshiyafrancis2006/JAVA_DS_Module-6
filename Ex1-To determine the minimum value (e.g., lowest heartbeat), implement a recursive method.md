# EX 1 – Recursive Minimum Finder (Health Monitoring Device)

### Date
11.11.2025  

### Developed by
## Name: Selshiya F 
## Register Number: 212224060241

---

##  Aim
To write a Java program to determine the minimum value (e.g., lowest heartbeat) using a recursive method.

---

## Algorithm
1. Start the program.  
2. Read the number of elements and store them in an array.  
3. Define a recursive function `findMin()` that compares elements to find the minimum.  
4. Base condition: If the array has one element, return that element.  
5. Recursive step: Compare the last element with the minimum of the rest of the array and return the smaller one.  
6. Display the minimum value.  
7. Stop the program.  

---

##  Program
```java
/**
 * Program: Determine the minimum value (e.g., lowest heartbeat) using recursion
 * Developed by: Selshiya F
 * Register Number: 212224060241
 */
import java.util.Scanner;

public class MinValueRecursive {
    static int findMin(int arr[], int n) {
        if (n == 1)
            return arr[0];
        return Math.min(arr[n - 1], findMin(arr, n - 1));
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter number of readings: ");
        int n = sc.nextInt();
        int arr[] = new int[n];
        System.out.println("Enter the readings:");
        for (int i = 0; i < n; i++)
            arr[i] = sc.nextInt();
        System.out.println("Minimum value (lowest heartbeat): " + findMin(arr, n));
        sc.close();
    }
}
```
## OUTPUT
<img width="938" height="161" alt="image" src="https://github.com/user-attachments/assets/4f716123-0d4a-4266-925d-c2fcac272460" />

## RESULT
Thus, the Java program to find the minimum value (e.g., lowest heartbeat) using a recursive method has been implemented successfully.
