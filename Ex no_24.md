# EX 24 Create a structure program to read(empno,dept and basic pay) and store the data of 3 employees and calculate their Gross Salary(da =10% and HRA=30% from BP).
## DATE: 11/05/2025
## AIM:
To Create a structure program to read(empno,dept and basic pay) and store the data of 3 employees and calculate their Gross Salary(da =10% and HRA=30% from BP).

## Algorithm
1.Start the program and define a structure with fields for employee number (empno), department (dept), and basic pay (basicPay).

2.Declare an array of structures to store the data of 3 employees.

3.Read the details (employee number, department, and basic pay) for each employee from the user.

4.Calculate the gross salary as: Gross Salary = Basic Pay + DA + HRA, where DA = 10% and HRA = 30% of the basic pay.

5.Display the details of each employee along with the calculated gross salary.
## Program:
```
/*
A structure program to read(empno,dept and basic pay) and store the data of 3 employees and calculate their Gross Salary(da =10% and HRA=30% from BP).
Developed by: Kamalesh S
RegisterNumber:  212223060108
*/
#include <stdio.h>

struct Employee
{
    int empno;
    char dept[50];
    float basicPay;
    float grossSalary;
};

int main()
{
    struct Employee emp[3];  // Array of structure to store data of 3 employees
    int i;

    for(i = 0; i < 3; i++)
    {
        printf("Enter details for employee %d:\n", i + 1);

        printf("Employee Number: ");
        scanf("%d", &emp[i].empno);

        printf("Department: ");
        scanf("%s", emp[i].dept);

        printf("Basic Pay: ");
        scanf("%f", &emp[i].basicPay);

        // Calculate DA and HRA
        float da = 0.10 * emp[i].basicPay;
        float hra = 0.30 * emp[i].basicPay;

        // Calculate Gross Salary
        emp[i].grossSalary = emp[i].basicPay + da + hra;

        printf("\n");
    }

    // Display employee details along with gross salary
    printf("Employee Details and Gross Salary:\n");
    for(i = 0; i < 3; i++)
    {
        printf("Employee %d: EmpNo = %d, Department = %s, Basic Pay = %.2f, Gross Salary = %.2f\n", 
               i + 1, emp[i].empno, emp[i].dept, emp[i].basicPay, emp[i].grossSalary);
    }

    return 0;
}

```

## Output:

![image](https://github.com/user-attachments/assets/442f3e4a-1d75-482c-8945-7feae6481320)


## Result:
Thus the program was executed and the output was verified successfully.
