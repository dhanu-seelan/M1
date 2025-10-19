
# EX-01-Datatypes-Operators
## AIM:
Write a C program to read 3 characters one by one and print the characters in a reverse order.

## ALGORITHM:
1.	Declare three character variables to store the input characters.
2.	Use the scanf function to read the characters one by one from the user.
3.	Print the characters in reverse order using the printf function.
4.	End the program.

## PROGRAM:

```
#include<stdio.h>
int main()
{
    char c1,c2,c3;
    scanf("%c %c %c",&c1 , &c2 , &c3);
    printf("%c %c %c",c3, c2, c1);
    return 0;
    
}

```
## OUTPUT:

<img width="1903" height="972" alt="image" src="https://github.com/user-attachments/assets/57064cdf-781b-47d6-8749-94992136151f" />
















## RESULT:
Thus the program to read 3 characters one by one and print the characters in a reverse order has been executed successfully.


# EX-02- Conditional-Statements
## AIM:
Write a C program to read A values and check whether A is positive number or not.

# ALGORITHM:
1.	Declare a variable to store the input value A.
2.	Use the scanf function to read the value of A from the user.
3.	Check if the value of A is greater than zero.
4.	If A is greater than zero, print a message indicating that it's a positive number. 
5.	Otherwise, print a message indicating that it's not a positive number.
6.End the program.

# PROGRAM:
```
#include<stdio.h>
int main()
{
    int A;
    scanf("%d",&A);
    if(A>0)
    {
        printf("It's a positive number");
    }
    else
    {
        printf("It's not a positive number");
    }
    return 0;
}
```
# OUTPUT:
<img width="1787" height="959" alt="image" src="https://github.com/user-attachments/assets/b57e9337-8aab-43f4-bd7c-cedcec0f9bad" />
<img width="1819" height="977" alt="image" src="https://github.com/user-attachments/assets/cbb9ea23-dcc5-4bd1-b196-a275009ffe34" />












# RESULT:
Thus the program to read A values and check whether A is positive number or not has been executed successfully.
 
 
 


# EX-03- Operators-Expressions
## AIM:
Write a program to find minimum between two fraction numbers using conditional operator or ternary operator.

## ALGORITHM:
1.	Declare variables to store the two fraction numbers and the result.
2.	Use the printf function to prompt the user to enter the first fraction number (numerator and denominator separately).
3.	Use the scanf function to read the numerator and denominator of the first fraction.
4.	Repeat steps 2 and 3 to get the second fraction from the user.
5.	Calculate the decimal values of both fractions by dividing the numerators by the denominators.
6.	Use the conditional (ternary) operator to compare the decimal values and store the minimum value in the result variable.
7.	Print the minimum value.

## PROGRAM:
```
#include<stdio.h>
int main()
{
    float num1,den1,num2,den2;
    float val1,val2,res;
    
    printf("First fraction: ");
    scanf("%f %f",&num1 , &den1);
    
    printf("Second fraction: ");
    scanf("%f %f",&num2 , &den2);
    
    val1=num1/den1;
    val2=num2/den2;
    
    res=(val1<val2)? val1:val2;
    printf("The minimum fraction is : %.4f",res);
    return 0;
    
}
```
## OUTPUT:

<img width="1896" height="961" alt="image" src="https://github.com/user-attachments/assets/40d128c3-0761-40e3-9dd3-3e048b7fb78a" />








## RESULT:
Thus the program to find minimum between two fraction numbers using conditional operator or ternary operator has been executed successfully.




# EX-04- Using Conditional Statements

## AIM:
Write a C program to check whether the input value is equal to 1 using simple if statement

## ALGORITHM:
1.	Declare a variable to store the input value.
2.	Use the scanf function to read the input value from the user.
3.	Use an if statement to check if the input value is equal to 1.
4.	If the condition in the if statement is true, print a message indicating that the input value is equal to 1.
5.	Otherwise, print a message indicating that it's not equal to 1.
6.	End the program.

## PROGRAM:
```
#include<stdio.h>
int main()
{
    int n;
    scanf("%d",&n);
    if(n==1)
    {
        printf("The number is equal to 1");
    }
    else
    {
        printf("The number is not equal to 1");
    }
    return 0;
}
```

## OUTPUT:
<img width="1844" height="965" alt="image" src="https://github.com/user-attachments/assets/6316c22a-53a0-407d-a176-d89e996bec4b" />
<img width="1796" height="963" alt="image" src="https://github.com/user-attachments/assets/f4c32dd4-0741-4486-9a06-4504763bef30" />










	

## RESULT:
Thus the program to check whether the input value is equal to 1 using simple if statement has been executed successfully



# EX-05- Calculating Total, Percentage, And Division Using Conditional Statements 
## AIM:
To write a C program that reads marks of three subjects, calculates the total and percentage, and then determines the division (First, Second, Pass, or Fail) based on the percentage and minimum marks criteria.
## ALGORITHM:
1.	Start
2.	Declare integer variables m1, m2, m3 for marks, and float variables tot, per.
3.	Input the marks for three subjects.
4.	Calculate total marks: tot = m1 + m2 + m3
5.	Calculate percentage: per = tot / 3
6.	Display total and percentage.
7.	Check if all marks are greater than or equal to 40:
8.	If yes:
a.	If percentage >= 60: Print “Division = First”
b.	Else if percentage >= 48: Print “Division = Second”
c.	Else if percentage >= 36: Print “Division = Pass”
9.	Else: Print “Division = Fail”
10.	End
## PROGRAM:
```
#include<stdio.h>
int main()
{
    int mark1,mark2,mark3;
     float tot,per;
    scanf("%d %d %d",&mark1, &mark2, &mark3);
    
    tot=mark1+mark2+mark3;
    per=tot/3;
    
    printf("Total Marks: %.2f\n",tot);
    printf("Percentage: %.2f\n",per);
    
    if(mark1>40 && mark2>40 && mark3>40)
    {
        if(per>=60)
        {
              printf("Division = First\n");
        }
        else if (per >= 48)
        {
            printf("Division = Second\n");
        }
        else if (per >= 36)
        {
            printf("Division = Pass\n");
        }
        else
        {
            printf("Division = Fail\n");
        }
    }
    else
    {
         printf("Division = Fail\n");
    }
    return 0;
    
}
```
## OUTPUT:
<img width="1840" height="957" alt="image" src="https://github.com/user-attachments/assets/89af5f4e-58e7-44b6-b46d-a498a559e0c2" />
<img width="1920" height="957" alt="image" src="https://github.com/user-attachments/assets/78b9373b-ef54-4b62-a18f-26d2368a899e" />
<img width="1856" height="961" alt="image" src="https://github.com/user-attachments/assets/8316d93e-f496-4d11-9741-1b95754cf692" />
<img width="1907" height="966" alt="image" src="https://github.com/user-attachments/assets/6d8787a4-c544-4531-a2a0-f94750b04005" />





## RESULT:
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.

