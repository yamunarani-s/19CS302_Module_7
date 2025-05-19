# EX 33 C program to read a file name from user and create that file using fopen().
## DATE:19/05/25
## AIM:
To write a C program to read a file name from user and create that file using fopen().

## Algorithm
 1. Analyze the question
2. Follow the algorithm
3. Try the code
4.  Check for error
5. Run & Display the output
## Program:
```
/*
C program to read a file name from user and create that file using fopen().
Developed by: 
RegisterNumber:  
*/
```
#include <stdio.h>

int main() {
    char filename[100];
    FILE *fp;
    scanf("%99s", filename);
    fp = fopen(filename, "w");
    if (fp == NULL) {
        printf("Error creating file '%s'\n", filename);
        return 1;
    }

    printf("File '%s' created successfully.\n", filename);

    fclose(fp);
    return 0;
}

## Output:
'File 'testfile.txt' created successfully.'


## Result:
Thus the program was executed and the output was verified successfully.
