# EXPERIMENT 07: WRITE A JAVA PROGRAM TO INSERT AN ELEMENT INTO AN ARRAY
## AIM:
To insert an element into an array using java programming language.
## PROCEDURE:
1. Import required packages.
2. Declare main method with the signature "public static void main(String[] args)".
3. Declare array and enter the elemnts.
4. Get the input from user for the position of intesertion.
5. Get the element that is to ber inserted.
6. Display the array after insertion.
7. End the program.


## PROGRAM:
```
import java.util.*;
public class Array {
    public static void main(String[] args)
    {
        int n, pos, x;
        Scanner s = new Scanner(System.in);
        System.out.print("Enter no. of elements you want in array:");
        n = s.nextInt();
        int a[] = new int[n+1];
        System.out.println("Enter all the elements:");
        for(int i = 0; i < n; i++)
        {
            a[i] = s.nextInt();
        }
        System.out.print("Enter the position where you want to insert element:");
        pos = s.nextInt();
        System.out.print("Enter the element you want to insert:");
        x = s.nextInt();
        for(int i = (n-1); i >= (pos-1); i--)
        {
            a[i+1] = a[i];
        }
        a[pos-1] = x;
        System.out.print("After inserting:");
        for(int i = 0; i < n; i++)
        {
            System.out.print(a[i]+",");
        }
        System.out.print(a[n]);
    }

}
```

## OUTPUT:
![image](https://github.com/Rithigasri/Experiment07-Java/assets/93427256/f34ef51f-b33d-42db-8d3e-1fb99498a6d1)

## RESULT:
Hence,a java program to insert an element into array is executed successfully.
