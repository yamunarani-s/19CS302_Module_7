# EX 31 C program to find the smallest among three numbers using Structure.
## DATE:19/05/25
## AIM:
To write a C program to find the smallest among three numbers using Structure.

## Algorithm
1. Analyze the question
2. Follow the algorithm
3. Try the code
4.  Check for error
5. Run & Display the output 

## Program:
```
/*
C program to find the smallest among three numbers using Structure.
Developed by: 
RegisterNumber:  
*/
```
#include <stdio.h>

// Define a structure to hold three numbers
struct Numbers {
    int num1;
    int num2;
    int num3;
};

// Function to find the smallest number
int findSmallest(struct Numbers n) {
    int smallest = n.num1;

    if (n.num2 < smallest) {
        smallest = n.num2;
    }
    if (n.num3 < smallest) {
        smallest = n.num3;
    }

    return smallest;
}

int main() {
    struct Numbers n;
    scanf("%d %d %d", &n.num1, &n.num2, &n.num3);

    // Find and display the smallest number
    int smallest = findSmallest(n);
    printf("Smallest number is: %d\n", smallest);

    return 0;
}
## Output:
'Smallest number is: 9'


## Result:
Thus the program was executed and the output was verified successfully.
