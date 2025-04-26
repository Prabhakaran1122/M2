# EX-06 - Looping
## AIM:
Write a C program to print even numbers ranging from M to N (including M and N values).

## ALGORITHM:
1.	Declare two integer variables to store the values of M and N.
2.	Use the printf function to prompt the user to enter the values of M and N.
3.	Use the scanf function to read the values of M and N from the user.
4.	Use a loop (for or while) to iterate from M to N.
5.	Inside the loop, check if the current number is even.
6.	If the current number is even, print it.
7.	Continue the loop until you have iterated through all numbers from M to N.

## PROGRAM:
```
#include <stdio.h>
int main() 
{
    int M, N;

    printf("Enter the value of M: ");
    scanf("%d", &M);

    printf("Enter the value of N: ");
    scanf("%d", &N);

    for (int i = M; i <= N; i++) {
        if (i % 2 == 0) {
            printf("%d ", i);
        }
    }

    return 0;
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/ca630048-5db4-4dc4-b89d-8bced844431a)











## RESULT:
Thus the program to print even numbers ranging from M to N (including M and N values) has been executed successfully
 
 


# EX-07-Nested-loop

## AIM:

Write a C program to print the given triangular pattern using loop.

## ALGORITHM:

1.	Declare a variable to store the number of rows in the triangle.
2.	Use the printf function to prompt the user to enter the number of rows.
3.	Use a loop (for or while) to iterate through each row.
4.	Inside the loop, use another loop to print the desired number of asterisks for each row.
5.	Continue the loop until you have printed the entire triangular pattern.

## PROGRAM:
```
#include <stdio.h>

int main() {
    int rows;

    printf("Enter the number of rows: ");
    scanf("%d", &rows);

    for (int i = 1; i <= rows; i++) {
        for (int j = 1; j <= i; j++) {
            printf("*");
        }
        printf("\n");
    }

    return 0;
}

```


## OUTPUT:

![image](https://github.com/user-attachments/assets/639e795f-f67e-4b13-b3b9-7b50e3b462ef)






## RESULT:

Thus the program to print the given triangular pattern using loop has been executed successfully
 
 


# EX-08-Functions

## AIM:

Write a C program to perform addition and subtraction of two numbers using functions (with argument and without return type).

## ALGORITHM:

1.	Declare two functions, one for addition and one for subtraction. Both functions should take two integer arguments.
2.	Inside the addition & subtraction function, add & subtract the two numbers and print the result.
3.	In the main function, declare two integer variables and read their values from the user.
4.	Call the addition and subtraction functions, passing the two numbers as arguments.

## PROGRAM:
```
#include <stdio.h>

void addition(int a, int b) {
    printf("Addition: %d\n", a + b);
}

void subtraction(int a, int b) {
    printf("Subtraction: %d\n", a - b);
}

int main() {
    int num1, num2;

    printf("Enter two numbers: ");
    scanf("%d %d", &num1, &num2);

    addition(num1, num2);
    subtraction(num1, num2);

    return 0;
}

```


## OUTPUT:
![image](https://github.com/user-attachments/assets/c7879ca5-1bbf-45fa-b9e1-a6ec4bc99679)







## RESULT:

Thus the program to perform addition and subtraction of two numbers using functions has been executed successfully
 
 


# EX-09-Use For Loop

## AIM:

Write a c program to find the sum of odd digits using for loop

## ALGORITHM:

1.	Declare variables to store the input number and the sum of odd digits.
2.	Initialize the sum of odd digits to 0.
3.	Use a for loop to iterate through each digit of the input number.
4.	Inside the loop, extract the rightmost digit of the number (using the modulo operator % and division by 10).
5.	If the digit is odd, add it to the sum of odd digits.
6.	Print the sum of odd digits.

## PROGRAM:
```
#include <stdio.h>

int main() {
    int start, n, sum = 0;

    printf("Enter the starting value: ");
    scanf("%d", &start);

    printf("Enter the value of n: ");
    scanf("%d", &n);

    for (int i = start; i <= n; i++) {
        if (i % 2 != 0) {
            sum += i;
        }
    }

    printf("Sum of odd numbers from %d to %d: %d\n", start, n, sum);

    return 0;
}


```


## OUTPUT:
![image](https://github.com/user-attachments/assets/89277721-ef99-4a5d-9a80-f5d2736fa0f0)





## RESULT:

Thus the program to find the sum of odd digits using for loop has been executed successfully.




# EX – 10 - Factorial of a Number Using a Function
## AIM:
To write a C program that calculates the factorial of a given number using a user-defined function.
## ALGORITHM:
1.	Start
2.	Declare the function fact().
3.	In the main() function, call the fact() function.
4.	In fact() function:
a.	Declare variables i, N, and fact (initialized to 1).
b.	Read an integer N from the user.
c.	Use a for loop from 1 to N:
i.	Multiply fact by i in each iteration.
d.	After the loop, print the factorial value.
5.	End

## PROGRAM:
```
#include <stdio.h>
int fact(int N) {
    int i, fact = 1;
    for (i = 1; i <= N; i++) {
        fact *= i;
    }
    return fact;
}

int main() {
    int N, result;

    printf("Enter a number: ");
    scanf("%d", &N);

    result = fact(N);

    printf("Factorial of %d is: %d\n", N, result);

    return 0;
}
```


## OUTPUT:
![image](https://github.com/user-attachments/assets/bb145a0a-a967-4f4f-91a0-8760006a4cf4)


## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
