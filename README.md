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
#include<math.h>
void emi(int p,float r,float t){
    float f;
    r=r/(12*100);
    t=t*12;
    f=(p*r*pow(1+r,t))/(pow(1+r,t)-1);
    printf("Monthly EMI is= %.3f",f);
}
int main(){
    int p;
    float r,t;
    scanf("%d %f %f",&p,&r,&t);
    emi(p,r,t);
}
```
## OUTPUT
![Screenshot 2025-04-30 205924](https://github.com/user-attachments/assets/8155ff44-3ef9-4166-b231-de5abd1cf698)





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
    int n,a=0,b=1,s=0;
    scanf("%d",&n);
    printf("%d ",a);
    printf("%d ",b);
    for (int i=0;i<=n-3;i++)
    {
        s=a+b;
        printf("%d ",s);
        a=b;
        b=s;
    }
}
```
## OUTPUT
![Screenshot 2025-04-30 210523](https://github.com/user-attachments/assets/1a7e55a8-6188-4a0e-87b0-09f5730a7e88)


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
        printf("%d ",a[n-1]);

    return 0;
}
```
## OUTPUT
![Screenshot 2025-04-30 210933](https://github.com/user-attachments/assets/efea4f2e-4110-4f6c-a236-52c5df55bdb5)



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
    int n, i, x, count = 0;
    printf("Enter number of elements: ");
    scanf("%d", &n);

    printf("Enter %d numbers: ", n);
    for(i = 0; i < n; i++) {
        scanf("%d", &x);
        if(x % 2 == 0)
            count++;
    }

    printf("Count of numbers divisible by 2 = %d\n", count);
    return 0;
}
```

## OUTPUT
![Screenshot 2025-04-30 211247](https://github.com/user-attachments/assets/5813a69e-7b9e-4186-b496-87b0fd4d7596)



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
    int n, i, arr[100];
    printf("Enter array size: ");
    scanf("%d", &n);

    printf("Enter %d elements: ", n);
    for(i = 0; i < n; i++)
        scanf("%d", &arr[i]);

    printf("Updated array: ");
    for(i = 0; i < n; i++) {
        if(arr[i] % 2 == 0)
            printf("E ");
        else
            printf("%d ", arr[i]);
    }

    return 0;
}
```
## Output:
 ![Screenshot 2025-04-30 211445](https://github.com/user-attachments/assets/8404a8db-f59a-4e26-be98-b040ad8dff99)


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



