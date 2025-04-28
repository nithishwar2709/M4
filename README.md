# EX-16-LEFT-SHIFT-OPERATION
## AIM
To write a C Program to perform the basic left shift operation for 44 integer number with 3 shifts.

## ALGORITHM
1.	Start the program.
2.	Assign values of a and b as 44 and 3.
3.	Use left shift operator (<<) and shift the value of a three times.
4.	Display the result.
5.	Stop the program.

## PROGRAM
`````
#include <stdio.h>
int main() {
    unsigned int a=44 ;	
      int c = 0; 
    c = a << 3;    
   printf("After Left Shift Operation value of a is:%d\n", c );
}
``````

## OUTPUT


![image](https://github.com/user-attachments/assets/b4922d15-8371-4022-a425-5618ac563b71)







## RESULT
Thus the program to perform the basic left shift operation for 44 integer number with 3 shifts has been executed successfully.




 
 


# EX-17-TWO-NUMBERS-ARE-EQUAL-OR-NOT


## AIM

Write a C Program to check whether the two numbers are equal or not using simple if statement.

## ALGORITHM

1.	Start the program.
2.	Read two numbers.
3.	If first number is equal to second number, display both are equal.
4.	Otherwise display both are not equal.
5.	Stop the program.

## PROGRAM
``````
# include <stdio.h>
int main()
{
    int a,b;
    scanf("%d %d",&a,&b);
    if(a==b)
    {
        printf("Numbers are Equal");
    }
    else
    {
        printf("Numbers are not Equal");
    }
    return 0;
}

``````


## OUTPUT

![image](https://github.com/user-attachments/assets/6c83b4c0-07c1-47a6-82d0-d1ced9c56fe0)


           
## RESULT

Thus the program to check whether the two numbers are equal or not using simple if statement has been executed successfully
 
 


# EX-18-STRING-LOWERCASE-CONVERSION
## AIM
Write a C Program to convert the given string into lowercase.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using tolower( ) function convert the given string into its lowercase.
4.	Display the result.
5.	Stop the program.

## PROGRAM
``````
#include<stdio.h>
#include<ctype.h>
#include<string.h>
int main()
{
    char str[100];
    scanf("%s",str);
    printf("Lower case String is:");
    for(int i=0;i<strlen(str);i++)
    {
        printf("%c",tolower(str[i]));
    }
}
``````

## OUTPUT
![image](https://github.com/user-attachments/assets/2a6e93da-054b-468f-bf48-b2c2b00c9039)





## RESULT
Thus the program to convert the given string into lowercase has been executed successfully
 
 


# EX-19-COUNT-OF-WORDS-IN-A-STRING
## AIM
Write a C Program to count the total number of words in a given string using do While loop.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using for loop, inspect the string character by character.
4.	Whenever a space is encountered increment count by 1.
5.	Display the result.
6.	Stop the program.

## PROGRAM
`````
#include<stdio.h>
#include<string.h>
#include<ctype.h>
int main()
{
    char str[1000];
    int i=0,count=0;
    scanf("%[^\n]s",str);
   do
   {
       if((str[i]!=' ' && str[i]!= '\t'&& str[i]!='\0') && (str[i+1]== ' ' || str[i+1]== '\t' || str[i+1]=='\0'))
       {
           count++;
       }
       i++;
   }while(str[i]!='\0');
   printf("%d\n",count);
}
``````

## OUTPUT

![image](https://github.com/user-attachments/assets/5a3e8f62-4dc6-41ff-b332-6fc27c6eb879)




## RESULT
Thus the program to count the total number of words in a given string using do While loop has been executed successfully
 
 


# EX  -20 -COMPARING TWO STRINGS
## AIM
write a Program to compare two strings without using strcmp().
## ALGORITHM
Step 1: Start the program.
Step 2: Declare two character arrays c1 and c2 of size 100 to store the strings. Also, declare an integer variable
             flag and initialize it to 0, and i for indexing.      
Step 3: Read the first string c1 using scanf("%[^\n]", c1); — this reads input until a newline is encountered 
            (i.e., can include spaces).
Step 4: Read the second string c2 using scanf("%s", c2); — this reads input until a space or newline (i.e., no 
            spaces in the second string).
Step 5: Start comparing characters of both strings from index i = 0.
Step 6: Repeat the following while neither c1[i] nor c2[i] is '\0' (i.e., end of string):
•	If c1[i] is not equal to c2[i], set flag = 1.
•	Increment i by 1.
Step 7: After the loop, check the value of flag:
•	If flag == 0, print "strings are same".
•	Otherwise, print "strings are not same".
Step 8: End the program.

## PROGRAM
`````
# include <stdio.h>
int main()
{
    char str1[100],str2[100];
    int i=0,str=1;
    scanf("%s",str1);
    scanf("%s",str2);
    while(str1[i]!='\0' || str2[i] != '\0')
    {
        if(str1[i]!=str2[i])
        {
            str=0;
            break;
        }
        i++;
    }
    if(str)
    {
        printf("strings are same\n");
    }
    else
    {
        printf("strings are not same\n");
    }
    return 0;
}
``````

## OUTPUT
 ![image](https://github.com/user-attachments/assets/33673906-723e-47dc-bfe0-910b1dec38d7)


## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.

