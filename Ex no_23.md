# EX 23 C program to store and display the name, id, age and salary of an employee using structure(using array of structure).
## DATE: 11/05/2025
## AIM:
To write a C program to store and display the name, id, age and salary of an employee using structure(using array of structure).

## Algorithm
1.Start the program and declare an integer pointer for the array, and a variable for counting even elements.

2.Use calloc() to dynamically allocate memory for the array.

3.Read the number of elements and input the array values.

4.Traverse the array and count the even elements.

5.Display the total number of even elements. 

## Program:
```
/*
C program to store and display the name, id, age and salary of an employee using structure(using array of structure).
Developed by: Kamalesh S
RegisterNumber:  212223060108
*/
#include <stdio.h>

struct Employee
{
    char name[100];
    int id;
    int age;
    float salary;
};

int main()
{
    struct Employee emp[2];  // Array of structure to store details of 5 employees
    int i;

    for(i = 0; i < 2; i++)
    {
        printf("Enter details for employee %d:\n", i + 1);

        printf("Name: ");
        scanf("%s", emp[i].name);

        printf("ID: ");
        scanf("%d", &emp[i].id);

        printf("Age: ");
        scanf("%d", &emp[i].age);

        printf("Salary: ");
        scanf("%f", &emp[i].salary);

        printf("\n");
    }

    printf("Employee Details:\n");
    for(i = 0; i < 2; i++)
    {
        printf("Employee %d: Name = %s, ID = %d, Age = %d, Salary = %.2f\n", 
               i + 1, emp[i].name, emp[i].id, emp[i].age, emp[i].salary);
    }

    return 0;
}


```

## Output:

![image](https://github.com/user-attachments/assets/b75facbd-f631-4c19-8e2f-a7b96d13674b)


## Result:
Thus the program was executed and the output was verified successfully.
