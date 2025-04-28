# EX-11-EMI-CALCULATOR

## AIM

To write a program to prepare EMI calculator using function without return type and with arguments.

## ALGORITHM

1.	Start the program.
2.	Read principal amount, rate of interest and months.
3.	Pass these values as arguments to function.
4.	Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>
#include <math.h> // For pow() function

// Function to calculate and display EMI
void calculateEMI(float principal, float annualRate, int tenureMonths) {
    float monthlyRate, emi;
    
    // Calculate monthly interest rate
    monthlyRate = annualRate / (12 * 100);
    
    // Calculate EMI
    emi = (principal * monthlyRate * pow(1 + monthlyRate, tenureMonths)) / (pow(1 + monthlyRate, tenureMonths) - 1);
    
    printf("\nEMI = %.2f\n", emi);
}

int main() {
    float principal, annualRate;
    int tenureMonths;
    
    // Input values
    printf("Enter Principal amount: ");
    scanf("%f", &principal);
    
    printf("Enter Annual Interest Rate (in %%): ");
    scanf("%f", &annualRate);
    
    printf("Enter Loan Tenure (in months): ");
    scanf("%d", &tenureMonths);
    
    // Call EMI calculation function
    calculateEMI(principal, annualRate, tenureMonths);
    
    return 0;
}
```

## OUTPUT


![image](https://github.com/user-attachments/assets/649cd2af-bcc2-4927-bd5f-5ec6c87a6f13)


## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 


# EX-12-FIBONACCI-SERIES

## AIM
To write a C program to generate the Fibonacci series for the value 6.

## ALGORITHM
1.	Start the program.
2.	Read number of terms to display.
3.	Add the previous two terms and store it in new term.
4.	Assign 2nd term to 1st term and 3rd term to 2nd term.
5.	Repeat steps 3 and 4 n number of times.
6.	Display the result.
7.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int n = 6; // Number of terms
    int a = 0, b = 1, next, i;
    
    printf("Fibonacci Series for %d terms:\n", n);
    
    for(i = 1; i <= n; i++) {
        printf("%d ", a);
        next = a + b;
        a = b;
        b = next;
    }
    
    return 0;
}
```
## OUTPUT
![image](https://github.com/user-attachments/assets/3da7569a-60e1-45da-8728-5b21e8723223)



## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.
 
 


# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the last element of the array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	Print the last element.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int n;
    
    // Input the number of elements
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    
    int arr[n]; // Declare an array of size n
    
    // Input n elements
    printf("Enter %d elements:\n", n);
    for(int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    
    // Print the last element
    printf("The last element is: %d\n", arr[n - 1]);
    
    return 0;
}
```
## OUTPUT

![image](https://github.com/user-attachments/assets/89c36d2d-0f5d-46f7-ac9e-1641d4a988dd)


## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be divided by 2 then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    int n, count = 0;
    
    // Input the number of elements
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    
    int arr[n]; // Declare an array of size n
    
    // Input n elements
    printf("Enter %d elements:\n", n);
    for(int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    
    // Count positive elements
    for(int i = 0; i < n; i++) {
        if(arr[i] > 0) {
            count++;
        }
    }
    
    // Print the result
    printf("Total number of positive elements: %d\n", count);
    
    return 0;
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/7a9193e3-10fc-41bc-b48f-f27fcbd48efb)





## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.



# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Aim:
To write a C program to replace all even elements with 'E' in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the array.
2.	Iterate through the array:
 	For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
3.	Replace even elements with 'E':
     If an element is even, replace that element with the character 'E'.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:
```
#include <stdio.h>

int main() {
    int n;
    
    // Input the number of elements
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    
    // Declare the array
    int arr[n];
    
    // Input n elements
    printf("Enter %d elements:\n", n);
    for(int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    
    // Replace even elements with 'E'
    for(int i = 0; i < n; i++) {
        if(arr[i] % 2 == 0) {
            printf("E ");
        } else {
            printf("%d ", arr[i]);
        }
    }
    
    return 0;
}
```
## Output:
 ![image](https://github.com/user-attachments/assets/5e0aec43-de9f-4c97-ac6d-b1b1ba510df9)



## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



