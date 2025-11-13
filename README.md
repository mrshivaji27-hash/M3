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

void calculateEMI(float principal, float rate, int time);

int main() {
    float principal, rate;
    int time;

    printf("Enter the loan amount (Principal): ");
    scanf("%f", &principal);

    printf("Enter the annual interest rate (in %%): ");
    scanf("%f", &rate);

    printf("Enter the loan period (in years): ");
    scanf("%d", &time);

    calculateEMI(principal, rate, time);

    return 0;
}

void calculateEMI(float principal, float rate, int time) {
    float monthlyRate, emi;
    int months;

    monthlyRate = rate / (12 * 100);
    months = time * 12;

    emi = (principal * monthlyRate * pow(1 + monthlyRate, months)) / 
          (pow(1 + monthlyRate, months) - 1);

   
    printf("\nMonthly EMI = ₹%.2f\n", emi);
}
```


## OUTPUT
<img width="1918" height="913" alt="image" src="https://github.com/user-attachments/assets/59031d87-b890-440b-979a-b809026ed5cc" />






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
    int n,a=0,b=1,nt;
    printf("Enter number of terms:");
    scanf("%d",&n);
    if (n==1)
    {
        printf("0");
    }
    if(n>1)
    {
        printf("0 1 ");
    }
    for(int i=3;i<=n;i++)
    {
        nt=a+b;
        printf("%d ",nt);
        a=b;
        b=nt;
    }
    return 0;
}
```


## OUTPUT








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
  printf("enter number of elements:");
  scanf("%d",&n);
  int arr[n];
  for(int i=0;i<n;i++)
  {
      printf("Enter element:");
      scanf("%d",&arr[i]);
  }

printf("the last element is %d",arr[n-1]);
    return 0;
}
```

## OUTPUT
<img width="1918" height="905" alt="image" src="https://github.com/user-attachments/assets/fac5c5f5-c660-4b0c-a4e7-ca439408546d" />










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
  int n,count=0;
  printf("enter number of elements:");
  scanf("%d",&n);
  int arr[n];
  for(int i=0;i<n;i++)
  {
      printf("Enter element:");
      scanf("%d",&arr[i]);
      if(arr[i]>0)
      {
          count++;
      }
  }
  

printf("Total number of positive values are %d",count);
    return 0;
}
```


## OUTPUT






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
  int n,count=0;
  printf("enter number of elements:");
  scanf("%d",&n);
  int arr[n];
  for(int i=0;i<n;i++)
  {
      printf("Enter element:");
      scanf("%d",&arr[i]);
      if(arr[i]%2==0)
      {
          arr[i]='E';
      }
      
  }
  for(int i=0;i<n;i++)
  {
   if(arr[i]=='E')
   {
      printf("%c ",arr[i]);
   }
  else
    {
      printf("%d ",arr[i]);
    }
  }
    return 0;
}
```

## Output:
 <img width="1893" height="900" alt="image" src="https://github.com/user-attachments/assets/a0c6952f-886d-4ef6-8e2e-8efe6cb3f7d7" />



## Result:
Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



