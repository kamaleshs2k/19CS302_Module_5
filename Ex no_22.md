# EX 22 C program to count total number of even elements in an array using calloc().
## DATE: 11/05/2025
## AIM:
To write a C program to count total number of even elements in an array using calloc().

## Algorithm
1.Start the program and declare an integer pointer for the array, and a variable for counting even elements.

2.Use calloc() to dynamically allocate memory for the array.

3.Read the number of elements and input the array values.

4.Traverse the array and count the even elements.

5.Display the total number of even elements. 

## Program:
```
/*
C program to count total number of even elements in an array using calloc().
Developed by: Kamalesh S
RegisterNumber:  212223060108
*/
#include <stdio.h>
#include <stdlib.h>

int main()
{
    int *arr, n, i, count = 0;

    printf("Enter the number of elements: ");
    scanf("%d", &n);

    arr = (int*)calloc(n, sizeof(int));

    if(arr == NULL)  
    {
        printf("Memory allocation failed.\n");
        return 1;
    }

    printf("Enter the elements:\n");
    for(i = 0; i < n; i++)
    {
        scanf("%d", &arr[i]);
    }

    for(i = 0; i < n; i++)
    {
        if(arr[i] % 2 == 0)
        {
            count++;
        }
    }

    printf("Total number of even elements: %d\n", count);

    
    free(arr);

    return 0;
}


```

## Output:

![image](https://github.com/user-attachments/assets/06604a64-225b-470b-a5dc-f9f9382279d0)


## Result:
Thus the program was executed and the output was verified successfully.
