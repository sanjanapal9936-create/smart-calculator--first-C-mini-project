# smart-calculator--first-C-mini-project
# Smart Calculator in CMy first mini project in C programming.## Features- Addition- Subtraction- Multiplication- Division- Average- Even / Odd- Square- Cube## LanguageC## Concepts Used- Variables- Input / Output- Switch Case- If-Else- Arithmetic Operators## AboutThis is my first C programming mini project,created while learning the basics of C.


#include <stdio.h>

int main() {
    int choice;
    float a, b, c, result;

    printf("\n===== SMART CALCULATOR =====\n");
    printf("1. Addition\n");
    printf("2. Subtraction\n");
    printf("3. Multiplication\n");
    printf("4. Division\n");
    printf("5. Average\n");
    printf("6. Even / Odd\n");
    printf("7. Square\n");
    printf("8. Cube\n");
    printf("9. Exit\n");

    printf("\nEnter your choice: ");
    scanf("%d", &choice);

    switch(choice) {

        case 1:
            printf("Enter two numbers: ");
            scanf("%f %f", &a, &b);
            result = a + b;
            printf("Result = %.2f", result);
            break;

        case 2:
            printf("Enter two numbers: ");
            scanf("%f %f", &a, &b);
            result = a - b;
            printf("Result = %.2f", result);
            break;

        case 3:
            printf("Enter two numbers: ");
            scanf("%f %f", &a, &b);
            result = a * b;
            printf("Result = %.2f", result);
            break;

        case 4:
            printf("Enter two numbers: ");
            scanf("%f %f", &a, &b);
            result = a / b;
            printf("Result = %.2f", result);
            break;

        case 5:
            printf("Enter three numbers: ");
            scanf("%f %f %f", &a, &b, &c);
            result = (a + b + c) / 3;
            printf("Average = %.2f", result);
            break;

        case 9:
            printf("Thank you for using Smart Calculator!");
            break;

        default:
            printf("Invalid choice!");
    }

    return 0;
}
