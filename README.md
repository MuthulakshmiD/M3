### Name : Muthulakshmi D - 212223040122
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
void emi(float p,float ar,int y)
{
    float mr=ar/(12*100);
    int m=y*12;
    float r=(p*mr*pow(1+mr,m)/(pow(1+mr,m)-1));
    printf("Monthly EMI is= %.3f\n",r);
}
int main()
{
    float p=345000.80;
    float r=9.25;
    int t=4;
    emi(p,r,t);
    return 0;
}
```

## OUTPUT

![image](https://github.com/user-attachments/assets/0190489f-1cbb-4a1d-ac8e-3c77d84b6e5c)

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
    int n,f1=0,f2=1,f3;
    scanf("%d",&n);
    for(int i=1;i<=n;i++)
    {
        printf("%d ",f1);
        f3=f1+f2;
        f1=f2;
        f2=f3;
        
    }
    return 0;
}
```

## OUTPUT

![image](https://github.com/user-attachments/assets/a86b84db-6444-4dbe-8ca4-75e8a4ba16f7)

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
    
}
```
## OUTPUT

![image](https://github.com/user-attachments/assets/93f414b1-6f42-4154-bcc0-5414ba71ce48)

## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-ODD-ELEMENTS
## AIM
write a C Program to display the count of odd elements in an array.

## ALGORITHM
1.Read the number of elements n and declare an array of size n.
2.Input n elements into the array.
3.Initialize a counter variable count = 0.
4.Traverse the array and increment count for each element that is odd (a[i] % 2 != 0).
5.Print the value of count as the total number of odd elements.

## PROGRAM
```
#include <stdio.h>
int main()
{
    int n,count=0;
    scanf("%d",&n);
    int a[n];
    for(int i=0;i<n;i++)
    {
        scanf("%d",&a[i]);
    }
    for(int i=0;i<n;i++)
    {
        if(a[i]%2!=0)
        {
            count++;
        }
    }
    printf("Total odd elements: %d",count);
}
```

## OUTPUT

![image](https://github.com/user-attachments/assets/02082633-d5fd-4225-81d6-019a9c7dab75)

## RESULT
Thus the program to display the count of odd elements in an array has been executed successfully.

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
    int n, i;
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    int arr[n];
    printf("Enter %d integers:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    for (i = 0; i < n; i++) {
        if (arr[i] % 2 == 0) {
            arr[i] = 'E';
        }
    }
    printf("Modified array:\n");
    for (i = 0; i < n; i++) {
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
 
![image](https://github.com/user-attachments/assets/040ce88c-f8f5-486d-874f-a76e269dc934)


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



