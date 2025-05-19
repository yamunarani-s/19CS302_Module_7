# EX 35 C program to create a file named "Hospital.txt" and display messages on successful creation, opening, and closing of the file.
## DATE:19/05/25
## AIM:
To write a C program to create a file named "Hospital.txt" and display messages on successful creation, opening, and closing of the file.

## Algorithm
1. Analyze the question
2. Follow the algorithm
3. Try the code
4.  Check for error
5. Run & Display the output
## Program:
```
/*
C program to create a file named "Hospital.txt" and display messages on successful creation, opening, and closing of the file.
Developed by: 
RegisterNumber:  
*/
```
#include <stdio.h>

int main() {
    FILE *fp;

    // Create and open the file in write mode
    fp = fopen("Hospital.txt", "w");

    if (fp == NULL) {
        printf("Failed to create or open the file 'Hospital.txt'\n");
        return 1;
    }

    printf("'File 'Hospital.txt' created and opened successfully.'\n");

    // Close the file
    if (fclose(fp) == 0) {
        printf("'File 'Hospital.txt' closed successfully.'\n");
    } else {
        printf("Error closing the file 'Hospital.txt'\n");
    }

    return 0;
}

## Output:
'File 'Hospital.txt' created and opened successfully.'
'File 'Hospital.txt' closed successfully.'



## Result:
Thus the program was executed and the output was verified successfully.
