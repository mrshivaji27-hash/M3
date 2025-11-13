# EX-11-EMI-CALCULATOR

## Name : k.shivaji
## Register Number : 25018038

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
void calculateEMI(float p, float r, int t);

int main() {
    float p, r;
    int t;
    scanf("%f%f", &p,&r);
    scanf("%d", &t);
    calculateEMI(p,r,t);
    return 0;
}

void calculateEMI(float p, float r, int t) {
    float emi;
    emi = (p* r * pow(1 + r, t)) / (pow(1 + r, t) - 1);
    printf("Monthly EMI is: %.2f\n", emi);
}
```



## OUTPUT
![alt text](img1.png)



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
    int n = 6; 
    int a = 0, b= 1, next, i;
    for (i = 1; i <= n; i++) 
    {
        printf("%d ", a);
        next = a+b;  
        a = b;       
        b = next;         
    }
    printf("\n");
    return 0;
}
```

## OUTPUT
![alt text](img2.png)


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
    int n, i;
    scanf("%d", &n);
    int arr[n]; 
    for (i = 0; i < n; i++) 
    {
        scanf("%d", &arr[i]);
    }
    printf("The last element is: %d\n", arr[n-1]);
    return 0;
}
```

## OUTPUT
![alt text](img3.png)



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
    int n, i, count = 0;
    scanf("%d", &n);
    int arr[n]; 
    for (i = 0; i < n; i++) 
    {
        scanf("%d", &arr[i]);
    }

    for (i = 0; i < n; i++) {
        if (arr[i] > 0) 
        {
            count++;
        }
    }
    printf("Total number of positive elements = %d\n", count);
    return 0;
}
```


## OUTPUT
![alt text](img4.png)

## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.





 
 


# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Name : A SATHYA NARAYANAN
## Register Number : 25016804

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

int main() 
{
    int n, i;
    scanf("%d", &n);
    int arr[n]; 
    for (i = 0; i < n; i++) 
    {
        scanf("%d", &arr[i]);
    }
    for (i = 0; i < n; i++) 
    {
        if (arr[i] % 2 == 0) 
        {
            printf("E ");  
        } else 
        {
            printf("%d ", arr[i]);  
        }
    }
    printf("\n");
    return 0;
}
```

## Output:
 ![alt text](img5.png)


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.


