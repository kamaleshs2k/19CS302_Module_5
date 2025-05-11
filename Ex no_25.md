# EX 25 C program to check whether a given character is a vowel or consonant using pointer
## DATE:11/05/2025
## AIM:
To write a C program to check whether a given character is a vowel or consonant using pointer

## Algorithm
1.Start the program and declare a character variable and a pointer.

2.Read a character from the user.

3.Use the pointer to access the character and check if it is a vowel (a, e, i, o, u).

4.If the character is a vowel, display "Vowel", otherwise, display "Consonant".

5.End the program. 

## Program:
```
/*
C program to check whether a given character is a vowel or consonant using pointer
Developed by: Kamalesh S
RegisterNumber:  212223060108
*/
#include <stdio.h>

int main()
{
    char ch;
    char *ptr = &ch;

    printf("Enter a character: ");
    scanf("%c", ptr);  // Read the character using the pointer

    // Check if the character is a vowel or consonant
    if(*ptr == 'a' || *ptr == 'e' || *ptr == 'i' || *ptr == 'o' || *ptr == 'u' || 
       *ptr == 'A' || *ptr == 'E' || *ptr == 'I' || *ptr == 'O' || *ptr == 'U')
    {
        printf("Vowel\n");
    }
    else
    {
        printf("Consonant\n");
    }

    return 0;
}


```

## Output:

![image](https://github.com/user-attachments/assets/39a04d48-270f-45c5-a79f-ad6652743ace)


## Result:
Thus the program was executed and the output was verified successfully.
