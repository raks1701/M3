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
void calculateEMI(double principal, double rate, int months) {
rate = rate / (12 * 100);
double emi = (principal * rate * pow(1 + rate, months)) / (pow(1 +
rate, months) - 1);
printf("The EMI for the loan is: %.2f\n", emi);
}
int main() {
double principal, rate;
int months;
scanf("%lf", &principal);
printf("Enter the principal amount: %.lf\n",principal);
scanf("%lf", &rate);
printf("Enter the annual rate of interest: %.lf\n",rate);
scanf("%d", &months);
printf("Enter the number of months: %d\n",months);
calculateEMI(principal, rate, months);
return 0;
}
```


## OUTPUT




![m-1 (2)](https://github.com/user-attachments/assets/2b142c50-c1e6-4bb2-98b8-97d297f774f6)

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
int main()
{
int n = 6;
int first = 0, second = 1, next;
printf("Fibonacci Series: %d %d ", first, second);
for (int i = 3; i <= n; i++) {
next = first + second;
printf("%d ", next);
first = second;
second = next;
}
printf("\n");
return 0;
}
```
## OUTPUT






![m-2 (2)](https://github.com/user-attachments/assets/2698db54-4610-48cb-b315-630cc19d1ab1)


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
scanf("%d", &n);
printf("Enter the number of elements: %d\n",n);
int arr[n];
printf("Enter %d elements:", n);
for (int i = 0; i < n; i++) {
scanf("%d ", &arr[i]);
}
for (int i = 0; i < n; i++) {
printf("%d ", arr[i]);
}
printf("\nThe last element is: %d\n", arr[n - 1]);
return 0;
}
```
## OUTPUT






![m-3 (2)](https://github.com/user-attachments/assets/0deeafdb-658a-438d-8b82-77d4dfc1d986)



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
int main() {
int n, count = 0;
scanf("%d", &n);
printf("Enter the number of elements: %d\n",n);
int arr[n];
printf("Enter %d elements:", n);
for (int i = 0; i < n; i++) {
scanf("%d", &arr[i]);
printf("%d ", arr[i]);
}
for (int i = 0; i < n; i++) {
if (arr[i] > 0) {
count++;
}
}
printf("\nTotal number of positive elements: %d\n", count);
return 0;
}
```

## OUTPUT




![m-4 (3)](https://github.com/user-attachments/assets/00bf7874-05d9-4d1c-867e-b679c5941a16)

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
printf("Enter the size of the array: %d\n",n);
int arr[n];
printf("Enter %d elements:", n);
for (int i = 0; i < n; i++) {
scanf("%d", &arr[i]);
printf("%d ", arr[i]);
}
for (int i = 0; i < n; i++) {
if (arr[i] % 2 == 0) {
arr[i] = 'E';
}
}
printf("\nUpdated array:");
for (int i = 0; i < n; i++) {
if (arr[i] == 'E') {
printf("E ");
} else {
printf("%d ", arr[i]);
}
}
return 0;
}
```
## Output:
 
![m-5 (3)](https://github.com/user-attachments/assets/2f6b4ddf-bd0d-4c7a-b588-ea3a65554506)

## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



