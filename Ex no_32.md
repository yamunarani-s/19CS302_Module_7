# EX 32 C program to display Hardware details such as price, product name and price using structure.
## DATE: 19/05/25
## AIM:
To write a C program to display Hardware details such as price, product name and price using structure.

## Algorithm
1. Analyze the question
2. Follow the algorithm
3. Try the code
4.  Check for error
5. Run & Display the output


## Program:
```
/*
C program to display Hardware details such as price, product name and price using structure.
Developed by: 
RegisterNumber:  
*/
```
#include <stdio.h>

// Define structure for hardware details
struct Hardware {
    char productName[50];
    float price;
};

int main() {
    struct Hardware hw;
    fgets(hw.productName, sizeof(hw.productName), stdin);

    // Remove newline character from fgets if present
    size_t len = 0;
    while (hw.productName[len] != '\0') {
        if (hw.productName[len] == '\n') {
            hw.productName[len] = '\0';
            break;
        }
        len++;
    }

    scanf("%f", &hw.price);

    // Display hardware details
    printf("\nHardware Details:\n");
    printf("Product Name: %s\n", hw.productName);
    printf("Price: %.2f\n", hw.price);

    return 0;
}


## Output:

'Hardware Details:'
'Product Name: Mouse'
'Price: 499.99'

## Result:
Thus the program was executed and the output was verified successfully.
