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

```C

#include <stdio.h>
#include <math.h>
int main()
{
    float principal, annual_rate, time;
    printf("Enter Principal Amount , Annual Rate and Time Peroid : ");
    scanf("%f %f %f",&principal,&annual_rate,&time);
    float monthly_interest = annual_rate/(12*100);
    float N=time*12;
    float EMI=(principal*monthly_interest*pow(1+monthly_interest,N))/(pow(1+monthly_interest,N)-1);
    printf("Monthly EMI is= %.3f",EMI);
}

```

## OUTPUT

![Screenshot 2025-04-30 001306](https://github.com/user-attachments/assets/13a20916-f01c-442b-b9ae-ba754e979059)

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

```C

#include<stdio.h>
int main()
{
    int n,first=1,second=-1,third=0;
    printf("Enter the number of terms to be displayed : ");
    scanf("%d",&n);
    printf("Fibbonachi Series for %d terms : ");
    for(int i=1;i<=n;i++)
    {
        third=first+second;
        printf("%d ",third);
        second=first;
        first=third;
    }
}

```

## OUTPUT

![Screenshot 2025-04-30 001849](https://github.com/user-attachments/assets/6c76158d-8713-463a-a72a-4d244ad2878c)

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


```C

#include<stdio.h>
int main()
{
    int n;
    printf("Enter the size of the array : ");
    scanf("%d",&n);
    int a[n];
    printf("Enter array elements : ");
    for(int i=0;i<n;i++)
    {
        scanf("%d ",&a[i]);
    }
    printf("%d",a[n-1]);
}

```

## OUTPUT

![Screenshot 2025-04-30 002444](https://github.com/user-attachments/assets/4e99747f-be5d-4c8e-92ca-81d7325eb7d7)

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

```C

#include<stdio.h>
int main()
{
    int n,pos=0;
    printf("Enter the size of the array : ");
    scanf("%d",&n);
    int a[n];
    printf("Enter array elements : ");
    for(int i=0;i<n;i++)
    {
        scanf("%d ",&a[i]);
        if(a[i]%2==0)
        {
            pos++;
        }
    }
    printf("The no of positive values in the array : %d",pos);
}

```

## OUTPUT

![Screenshot 2025-04-30 004100](https://github.com/user-attachments/assets/38246bbb-70a7-4c63-96df-724155ed93ec)

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

```C

#include <stdio.h>
int main() 
{
    int size;
    printf("Enter the size of the array: ");
    scanf("%d", &size);
    int arr[size]; 
    printf("Enter %d elements:\n", size);
    for (int i = 0; i < size; i++) 
    {
        scanf("%d", &arr[i]);
    }
    printf("Updated array:\n");
    for (int i = 0; i < size; i++) 
    {
        if (arr[i] % 2 == 0) 
        {
            printf("E ");
        } 
        else 
        {
            printf("%d ", arr[i]);
        }
    }
    printf("\n");

    return 0;
}

```

## Output:
 
![Screenshot 2025-04-30 004331](https://github.com/user-attachments/assets/79698d65-1739-481d-a893-ef14ec56021e)

## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



