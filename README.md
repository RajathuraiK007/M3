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
#include<stdio.h>
#include<math.h>
void EMI(float P, float n, float r)
{
    r/=(12*100);
    float emi = (P*r*pow((1+r),n))/(pow(1+r,n)-1);
    printf("%.2f",emi);
}
int main()
{
    float P,n,r;
    scanf("%f %f %f",&P,&n,&r);
    EMI(P,n,r);
    return 0;
}


## OUTPUT
<img width="1812" height="715" alt="image" src="https://github.com/user-attachments/assets/915286d7-1aa1-440e-97ae-4abfb1eade55" />


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
#include<stdio.h>
int main()
{
    int n;
    scanf("%d",&n);
    int term_1=0,term_2=1;
    printf("%d %d ",term_1,term_2);
    for(int i=1;i<=n-2;i++)
    {
        int next_term=term_1+term_2;
        term_1=term_2;
        term_2=next_term;
        printf("%d ",next_term);
    }
    return 0;
}

## OUTPUT
<img width="1813" height="688" alt="image" src="https://github.com/user-attachments/assets/38b5e09f-545f-4fef-bb11-267155c50a84" />


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
#include<stdio.h>
int main()
{
    int n;
    scanf("%d\n",&n);
    int arr[n];
    for(int i=0;i<n;i++)
    {
        scanf("%d",&arr[i]);
    }
    printf("%d",arr[n-1]);
    return 0;
}

## OUTPUT
<img width="1337" height="712" alt="image" src="https://github.com/user-attachments/assets/e8319e1f-05a4-4665-bcc8-f6152587ecfa" />

## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS

## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value is greatar than then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM
#include<stdio.h>
int main()
{
    int n;
    scanf("%d\n",&n);
    int arr[n];
    for(int i=0;i<n;i++)
    {
        scanf("%d",&arr[i]);
    }
    int count=0;
    for(int i=0;i<n;i++)
    {
        if(arr[i]>=0)
        count++;
    }
    printf("%d",count);
    return 0;
}

## OUTPUT

<img width="1814" height="586" alt="image" src="https://github.com/user-attachments/assets/4d0274a4-6dfb-4f0a-a496-666ea05f3fea" />





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
#include<stdio.h>
int main()
{
    int n;
    scanf("%d",&n);
    int arr[n];
    for(int i=0;i<n;i++)
    {
        scanf("%d",&arr[i]);
    }
    for(int i=0;i<n;i++)
    {
        if(arr[i]%2==0)
        printf("E ");
        else
        printf("%d ",arr[i]);
    }
    return 0;
}

## Output:
 <img width="1813" height="604" alt="image" src="https://github.com/user-attachments/assets/5d1364cb-d626-4686-8a8f-3c2e821a03c1" />


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



