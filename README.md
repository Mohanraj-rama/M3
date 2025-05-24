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
#include <math.h>
void calculateEMI(float principal, float rate_of_interest, int months) {
    float monthly_rate = rate_of_interest / (12 * 100);
    float emi = (principal * monthly_rate * pow(1 + monthly_rate, months)) / (pow(1 + monthly_rate, months) - 1);
    printf("The EMI for the loan is: %.2f\n", emi);
}

int main() {
    float principal, rate_of_interest;
    int months;
    printf("Enter the principal amount: ");
    scanf("%f", &principal);
    
    printf("Enter the rate of interest (annual in percentage): ");
    scanf("%f", &rate_of_interest);
    
    printf("Enter the number of months: ");
    scanf("%d", &months);
    
    calculateEMI(principal, rate_of_interest, months);
    
    return 0;
}
```

## OUTPUT

![image](https://github.com/user-attachments/assets/378689f3-1a9a-4d30-ac64-386bd6ec6e80)




## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 


# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 8.

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
int main()
{
    int n,a=0,b=1;
    scanf("%d",&n);
    int i=1;
    do
    {
        printf("%d ",a);
        int c=a+b;
        a=b;
        b=c;
        i++;
    }while(i<=n);
    return 0;
}
```

## OUTPUT


![image](https://github.com/user-attachments/assets/b728c38c-a32c-4ab6-9de4-36c66f19f933)






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
int main()
{
    int n;
    scanf("%d",&n);
    int a[n];
    for(int i=0;i<n;i++)
    {
        scanf("%d",&a[i]);
    }
    printf("%d",a[n-1]);
    return 0;
}
```

## OUTPUT


![image](https://github.com/user-attachments/assets/7492e5ec-1d72-46fb-b370-8469e4824c62)







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
int main()
{
    int n,c=0;
    scanf("%d",&n);
    int a[n];
    for(int i=0;i<n;i++)
    {
        scanf("%d",&a[i]);
    }
    for(int j=0;j<n;j++)
    {
        if(a[j]>0)
        {
            c++;
        }
    }
    printf("count  of positive numbers  in array: %d",c);
    return 0;
}
```

## OUTPUT



![image](https://github.com/user-attachments/assets/f895162b-98ec-4228-8956-34b24fcc2bf6)


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
    scanf("%d", &n);
    int a[n];

    for (int i = 0; i < n; i++) {
        scanf("%d", &a[i]);
    }

    for (int i = 0; i < n; i++) {
        if (a[i] % 2 == 0) {
            printf("E ");
        } else {
            printf("%d ", a[i]);
        }
    }

    return 0;
}
```

## Output:

 ![image](https://github.com/user-attachments/assets/18cc5672-baa4-4d89-9a8e-080097a1d425)



## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



