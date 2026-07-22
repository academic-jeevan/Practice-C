# Practice-C
```
Hello World
#include <stdio.h>

int main() {
    printf("Hello World");

    return 0;
}

```
Vrialbles & Data Types

#include <stdio.h>

int main() {
    int age = 20;
    float height = 5.8;
    char grade = 'A';

    printf("Age = %d\n", age);
    printf("Height = %.1f\n", height);
    printf("Grade = %c\n", grade);

    return 0;
}

Input using
#include <stdio.h>

int main() {
    int age;

    printf("Enter your age: ");
    scanf("%d", &age);

    printf("Your age is %d", age);

    return 0;
}

Calculator
#include <stdio.h>

int main() {
    float num1, num2;

    printf("Enter first number: ");
    scanf("%f", &num1);

    printf("Enter second number: ");
    scanf("%f", &num2);

    printf("Addition = %.2f\n", num1 + num2);
    printf("Subtraction = %.2f\n", num1 - num2);
    printf("Multiplication = %.2f\n", num1 * num2);
    printf("Division = %.2f\n", num1 / num2);

    return 0;
}

if-else
#include <stdio.h>

int main() {
    int num;

    printf("Enter a number: ");
    scanf("%d", &num);

    if (num % 2 == 0) {
        printf("The number is Even");
    } else {
        printf("The number is Odd");
    }

    return 0;
}

switch-case (Simple Calculator)
#include <stdio.h>

int main() {
    float num1, num2;
    char operator;

    printf("Enter first number: ");
    scanf("%f", &num1);

    printf("Enter an operator (+, -, *, /): ");
    scanf(" %c", &operator);

    printf("Enter second number: ");
    scanf("%f", &num2);

    switch (operator) {
        case '+':
            printf("Result = %.2f", num1 + num2);
            break;

        case '-':
            printf("Result = %.2f", num1 - num2);
            break;

        case '*':
            printf("Result = %.2f", num1 * num2);
            break;

        case '/':
            printf("Result = %.2f", num1 / num2);
            break;

        default:
            printf("Invalid operator");
    }

    return 0;
}

for Loop (Print 1 to N)
#include <stdio.h>

int main() {
    int n, i;

    printf("Enter the value of N: ");
    scanf("%d", &n);

    for (i = 1; i <= n; i++) {
        printf("%d\n", i);
    }

    return 0;
}

while Loop (Reverse a Number)
#include <stdio.h>

int main() {
    int num, reverse = 0, remainder;

    printf("Enter a number: ");
    scanf("%d", &num);

    while (num != 0) {
        remainder = num % 10;
        reverse = reverse * 10 + remainder;
        num = num / 10;
    }

    printf("Reverse = %d", reverse);

    return 0;
}
