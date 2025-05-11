# EX 21 C program to calculate the area of a triangle using pointer.
## DATE:11/05/2025
## AIM:
To write a C program to calculate the area of a triangle using pointer.

## Algorithm
1.Start the program and declare three float variables for the base, height, and area of the triangle.

2.Declare a pointer for the area variable.

3.Read the base and height of the triangle from the user.

4.Use the pointer to calculate the area (Area = 0.5 * base * height).

5.Display the calculated area. 

## Program:
```
/*
C program to calculate the area of a triangle using pointer.
Developed by: Kamalesh S
RegisterNumber:  212223060108
*/
#include <stdio.h>

int main()
{
    float base, height, area;
    float *ptr = &area;  

    printf("Enter the base of the triangle: ");
    scanf("%f", &base);

    printf("Enter the height of the triangle: ");
    scanf("%f", &height);

    
    *ptr = 0.5 * base * height;

    printf("Area of the triangle: %.2f\n", *ptr);

    return 0;
}


```

## Output:

![image](https://github.com/user-attachments/assets/25caf876-f3f4-4f45-b7ef-c1a82fc1b17f)


## Result:
Thus the program was executed and the output was verified successfully.
