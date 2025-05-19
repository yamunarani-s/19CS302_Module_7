# EX 34 C program to read a file name from user and create that file and insert student roll numbers in to that file.
## DATE:19/05/25
## AIM:
To write a C program to read a file name from user and create that file and insert student roll numbers in to that file.

## Algorithm
1. Analyze the question
2. Follow the algorithm
3. Try the code
4.  Check for error
5. Run & Display the output
## Program:
```
/*
C program to read a file name from user and create that file and insert student roll numbers in to that file.
Developed by: 
RegisterNumber:  
*/
```
#include <stdio.h>

int main() {
    char filename[100];
    FILE *fp;
    int n, rollNumber;
    scanf("%99s", filename);
    fp = fopen(filename, "w");
    if (fp == NULL) {
        return 1;
    }
    scanf("%d", &n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &rollNumber);
        fprintf(fp, "%d\n", rollNumber);  // Write each roll number on a new line
    }

    printf("Student roll numbers successfully written to '%s'\n", filename);

    fclose(fp);
    return 0;
}

## Output:
101
102
103
'Student roll numbers successfully written to 'students.txt''


## Result:
Thus the program was executed and the output was verified successfully.
