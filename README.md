[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/Kc_5KWsV)
<div align="center"><img src="sust-logo.png" width="100"></div>

Question Setter
---------------
Name:  **Ali Ashraf Tanvir**         
Registration # **2021331001**            
Session: *2021-22*            
GitHub Username: *tanvir2021331001*               
Cell: *+8801706260318*              
Email: *aliashraftanvir410@gmail.com, 2021331001@student.sust.edu*         

Question Set with Answers
=========================

<h2 align="center">Shahjalal University of Science and Technology
</h2>
<h3 align="center">Department of Computer Science and Engineering
</h3>
<div align="center"> 1<sup>st</sup> Year 1<sup>st</sup> Semester Final Examination &mdash;
June 2022 (Session 2021-22) </div>
<div align="center"> Course No. &mdash; <b> CSE 133</b> </div>
<div align="center"> Course Title &mdash; <b> Structured Programming Language</b> </div>
<div align="center"> Time &mdash; <b>  3 Hours</b> &nbsp;&nbsp;&nbsp;&nbsp; Credit: <b> 3.00</b>&nbsp;&nbsp;&nbsp;&nbsp;Total Marks # <b> 100</b></div>
<hr class="divider">
<div align="center"> (Answer All the Questions)</div><br>
<div align="center"><b>Group A</b> </div>
<div align="left">1. Answer the following Questions in short. (Any <b>Five</b>). &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;5 &times; 2 = 10 </div>

(a) Lets,A 64 bit computer has a capacity of 50 M words.How many integer and character can be stored in the computer ?     
*Answer:*
<pre>
50 words equivalent to =50x1024x1024 words 
                       =52428800 words
The word is 64-bit or 8 byte 
So, The computer can store=52428800x8/4 integer or 104857600 integer
  
The computer can store=52428800x8=419430400 character
   </pre>     
 
(b)What is a symbolic constant? How is a symbolic constant defined?

Answer:
<p>
A symbolic constant is a name that substitutes for a sequence of characters. The characters may represent a numeric constant, a character constant or a string constant. Thus, a symbolic constant allows a name to appear in place of a numeric constant, a character constant or a string.                                   <br>

A symbolic constant is defined by writing <br>
#define name text                         <br>
where "name"represents a symbolic name, typically written in uppercase letters, and "text" represents the sequence of characters that is associated with the symbolic name.
</p>      
(c) What will be the output of the following program:

```c
#include<stdio.h>
int main(){
    int a=2,b=0,c=1,p=0;
    c=((a==b)?4+(++b):a+++--b- --c);
    printf("OUTPUT: a=%d c=%d b=%d\n",a,b++,c);
    return 0;
}
```

Answer:
```
OUTPUT: a=3 c=-1 b=1
```  
(d) What is the function of break and continue statement and what is the difference ?Answer the question in short.   <br>
Answer:
<p>
The function of the break statement is to exit or terminate a loop or switch statement prematurely.And The function of the continue statement is to skip the remaining code within a loop iteration and move to the next iteration.              <br>
In short, break allows for early termination of loops or switch statements, on the other hand continue allows for skipping the remaining code in a loop iteration and proceeding to the next iteration.
</p>      
(e)

```c
#include<stdio.h>
#include<string.h>
int main(){
    char b[]={"asdfg"};
    int x=sizeof(b),y;
    char a[15]={"op\nnm\0jf"};
    y=sizeof(b);
    printf("OUTPUT: x=%d y=%d \n",x,y);
    return 0;
}
```
*Is string.h header file mandatory for the program?Write the output of the program.*

Answer:
No,string.h header file is not important for the program.

```
OUTPUT: x=6 y=6
```
        
(f)You will be the values of a,b and c;Find the value of x form the equation of ax^2+bx+c=0 using c programming.
Answer:
*As it is a quadratic equation,the x has two value .So,we defined its values as x1 and x2.*
```c
#include<stdio.h>
#include<math.h>
int main(){
    int a,b,c;
    printf("Input(a b c): ");
    scanf("%d %d %d",&a,&b,&c);
    float x1,x2,d;
    d=sqrt(b*b-4*a*c);
    x1=(-b+d)/(2.0*a);
    x2=(-b-d)/(2.0*a);
    printf("OUTPUT: x1=%f x2=%f \n",x1,x2);
    return 0;
}
```
Sample:
```
Input(a b c): 1 6 2
OUTPUT: x1=-0.354249 x2=-5.645751 
 ```     
(g)Interpret the following statement :

scanf("%ld%5hd%15lf%11le", &a, &b, &c, &d);


Answer:
<p>
%ld: This format specifier is used to read a long integer from the input.    <br>

%5hd: This format specifier is used to read a short integer from the input with a field width of 5 characters.    <br>

%15lf: This format specifier is used to read a double precision floating-point number from the input with a field width of 15 characters. <br>

%11le: This format specifier is used to read a floating-point number in exponential format from the input with a field width of 11 characters.        <br>
&a, &b, &c, &d: These are the memory addresses where the values read from the input will be stored.

  </p>      
(h)10101101 00000101 it is the memory representation of 2 byte floating point number.here is 8 bits mantissa and 7 bits for exponent.
Reconstruct this number retrieving it from this memory representation.
<pre>
Answer:
Here 1st 1 bit is the sign bit.it is 1, so, The number is negative.Next 01011010 is mantissa and 0000101 is exponent
Exponent 0000101 is 4+0+1 =5
Therefore the memory representation will be(10110.1)<sub>2</sub>
Soothe number will be -(2^4+0+2^2+2^1+0+1/2)=(-22.5)<sub>10</sub>
</pre>

<div align="left">2. Answer the following Questions. (Any <b>Four</b>). &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4 &times; 5 = 20 </div>

(a) Write the output of the program.

```c
#include<stdio.h>
int main(){
int a,b,c,n,s;
scanf("%1d  %2d%d%d",&a,&b,&c,&n);
s=a+++b+c--;
printf("OUTPUT:a=%d b=%d c=%1d s=%2d\n",a,b,c,s,n);
return 0;
}
```
Input: 123456 78  <br>
Answer: 

*OUTPUT:a=2 b=23 c=455 s=480*
         
(b)What is Timesharing? Write down the desirable characteristics of a program.

Answer: 
<p>
Timesharing is a method that allows many different users to use a single computer simultaneously.
Desirable program characteristics:            <br>
(i) Integrity: It means the accuracy of the calculation. The full program will be meaningless if the calculation is not correct.<br>
(ii) Clarity: It refers readability of a program. The program logic must be clear so that other programmers can understand it without undue effort.<br>
(iii) Simplicity: The program must be simple as possible and the program should be straightforward to Objective.<br>
(iv) Efficiency: The program should be time and memory efficient.<br>
(v) Modularity: The large program should be divided into many subtasks or modules. Such as creating a function is preferable for large programs.<br>
(vi) Generality: The program should be as general as possible. For Example, we should use a key parameter rather than placing a fixed value.
 <p>      
(c)
  <p>"Tower of Hanoi" is a well-known children's game. Suppose your younger brother starts playing the game . But, when the number of disks is greater than 3, He fails the game. He asked you for instructions.You know that when the disk number is large the game will be difficult. So,as a coder, you should write a code for instruction. Please write a code for solving the game in C programming language.
  </p>

Answer:
```c
#include<stdio.h>
#include<string.h>
void toh(int n,char L,char R,char C){
   if(n>0){
 toh(n-1,L,C,R);
   
   printf("move %d th disc %c To %c\n",n,L,R);
   toh(n-1,C,R,L);
   }
      return;
}
int main(){
   int n;
  scarf("%d",&n);
  toh(n,'L','R','C');
   return 0;
}
```
        
(d) Following the code convert it to an if else statement.
```c
#include<stdio.h>
int main(){
    int i,j,k,x=0;
    for(i=0;i<5;++i){
        for(int j=0;j<i;++j){
         switch(i+j-1){
             case -1:
             case 0:
                   x+=1;
                   break;
             case 1:
             case 2:
             case 3:
                   x+=2;
                   break;
             default:
                   x+=3;
         } 
         printf("%d ",x);
         
        }
        printf("\nx=%d ",x);
    }
    return 0;
}
```

Answer:
```c
#include <stdio.h>

int main() {
    int i, j, k, x = 0;
    for (i = 0; i < 5; ++i) {
        for (j = 0; j < i; ++j) {
            if (i + j - 1 == -1 || i + j - 1 == 0) {
                x += 1;
            } else if (i + j - 1 == 1 || i + j - 1 == 2 || i + j - 1 == 3) {
                x += 2;
            } else {
                x += 3;
            }
            printf("%d ", x);
        }
        printf("\nx=%d ", x);
    }
    return 0;
}

```


          

<div align="left">3. Answer the following Questions. (Any <b>Two</b>). &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2 &times; 10 = 20 </div>

(a) *You are given a sample function and its plot :*
*y=x*
```
INPUT:
5
1 2 3 4 5

output:
|    .    
|   .     
|  .      
| .       
|.        
|_________
```

*Write a program which will make a plot by function y-x+1=0.The value of x and its number n will be Input.*
*And output will be a plot.[x<50,y<50,n<50]*

*Answer:*
```c
#include<stdio.h>
#include<stdlib.h>
#define R1 50
#define R2 50

 char a[R1+2][R2+2];
int main(){
      int n,max=-1,maxx=-1;
      printf("INPUT:\n");
      scanf("%d",&n);
      int x[n],y[n];
      for(int i=1;i<=n;i++)
      {
          scanf("%d",&x[i]);
          if(maxx<x[i])maxx=x[i];
          
          y[i]=x[i];
          if(max<y[i])max=y[i];
      }
      
      for(int i=0;i<=R1;i++)
      {
      a[i][0]='|';
      a[max][i]='_';
          
      }
    
    for(int i=1;i<=n;i++)
    { if(x[i]<0||y[i]<0);
    
      else a[max-y[i]][x[i]]='.';
    }
    printf("output:\n");
    for(int i=0;i<=max;i++)
    {
        for(int j=0;j<maxx+5;j++)
        {
            if(a[i][j]=='.'||a[i][j]=='_'||a[i][j]=='|'){
                printf("%c",a[i][j]);
            }
            
            else printf(" ");
        }
        printf("\n");
    }
    

    return 0;
}
```
<pre>
INPUT:         
5
1 3 4 5 6
output:    
|     .    
|    .     
|   .      
|  .       
|          
|._________

</pre>
         
(b) 
```c
#include<stdio.h>
typedef struct{
char nam[10];
int a;
}bn;
int main(){
int i,j,k,x=0;
bn su=("aspr",234);
printf("OUTPUT: \n");

 for(i=0;i<5;++i){
    for(int j=0;j<i;++j){
        switch(i+j-1){
           case -1:
           case 0:
                  x+=1;
                  break;
           case 1:
           case 2:
                  printf("%s %d\n",su->nam,su->a);
           case 3:
                 x+=2;
           default:
                  x+=3;
        }
    
     printf("%d ",x);
    }
  printf("x=%1d ",x);
 }
return 0;
}
```
*Is there any error in the program? Please rewrite the program without error if any. And write the output of the correct program.*

*Answer:*

*Yes, There are some error in the given program.In the line number 8,should be assign second bracket instead of using 1st bracket.*
*And in the line number 18 should be used '.' Instead of using '->'.Because su is not a pointer.*
*The correct program:*
```c
#include<stdio.h>
typedef struct{
char nam[10];
int a;
}bn;
int main(){
int i,j,k,x=0;
bn su={"aspr",234};
printf("OUTPUT: \n");
 for(i=0;i<5;++i){
    for(int j=0;j<i;++j){
        switch(i+j-1){
           case -1:
           case 0:
                  x+=1;
                  break;
           case 1:
           case 2:
                  printf("%s %d\n",su.nam,su.a);
           case 3:
                 x+=2;
           default:
                  x+=3;
        }
    
     printf("%d ",x);
    }
  printf("x=%1d ",x);
 }
return 0;
}
```
```
OUTPUT: 
x=0 1 x=1 aspr 234
6 aspr 234
11 x=11 aspr 234
16 21 24 x=24 29 32 35 38 x=38 
```
       
(c) 
*Kalu wrote a program that creat Pascale triangle,That works in the same manner: *
```
Number of rows:
4
OUTPUT: 
1
1 1
1 2 1
1 3 5 3 1
```
*He asked you to represent the triangle in a different way like an equilateral triangle.*
*So, write a program following such a condition.*

Answer:
```c
#include <stdio.h>
int main() {
   int n;
   printf("Number of rows: \n");
   scanf("%d",&n);
   printf("OUTPUT: \n");
   for(int i=1;i<=n;i++)
   {
       for(int j=1;j<=n-i;j++)
       {
           printf("   ");
       }
       int value=1;
       for(int j=1;j<=i;j++)
       {
           printf("%-6d",value);
           value=value*(i-j)/j;
           
       }
       printf("\n");
   }
   return 0;
}

```
```
Number of rows: 
10
OUTPUT: 
                           1     
                        1     1     
                     1     2     1     
                  1     3     3     1     
               1     4     6     4     1     
            1     5     10    10    5     1     
         1     6     15    20    15    6     1     
      1     7     21    35    35    21    7     1     
   1     8     28    56    70    56    28    8     1     
1     9     36    84    126   126   84    36    9     1    
```
       

<div align="center"><b>Group B</b> </div>
<div align="left">1. Answer the following Questions in short. (Any <b>Five</b>). &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;5 &times; 2 = 10 </div>

(a) What is the difference between #include<math.h> and #include"math.h"?  
Answer:            <br>
</p>
#include <math.h>: This syntax is used to include standard library header files.On the other hand, #include "math.h": This syntax is used to include user-defined or custom header files.       <br>
The angle brackets" < > " indicate that the header file is part of the standard library provided by the compiler and The double quotes " " indicate that the header file is located in the current directory or in a specified path relative to the current file. 
</p>
  
(b) Write  one statement for swapping two integers.
Answer:
<pre>
Lets, Two variable are a and b;
So, the statement is
a^=b^=a^=b;
</pre>

(c) Write the output of the program :
```c
#include<stdio.h>
#define bi <<
#define NoPrint(n) printf("bi Output:%d\n",n); \
        n=n bi 5
int main(){
    int k=3;
    NoPrint(k);
    NoPrint(k);
}
```
Answer:
```
bi Output:3
bi Output:96
  ```    
(d) is there any bug in the following code?if any fix it.And write the output.
```c
#include<stdio.h>
#define ret return 
#define display2(in) printf(#in "\n");
#define display1(p) printf(#p"=%d\n",p);
#define display3(a) a

int main(){
    int k=3;
    display1(k)
    display2(k) k++;
    
    k+=display3(k);
    display1(k);
    ret 0;
}
```
Answer:
No,there are no bug in the program.
Output:
```
k=3
k
k=8
 ```       
(e)What is the difference between structure and union?
<p>
A structure is a user-defined data type that allows you to group different types of variables under a single name.Each variable within a structure has its own memory space, and they can have different sizes and types.    <br>
On the other hand,A union is also a user-defined data type that allows you to group different types of variables under a single name, but they share the same memory space.
</p>
        
(f) Write a program for input and output in a file.
<p>
Input file(input.txt) : 100 integer with space.   <br>
Output file(output.txt): same integer with comma.  <br>
</p>
Answer:

```c
#include <stdio.h>

int main() {
    FILE *in;
    FILE *out;
    
    in= fopen("input.txt", "r");
    out = fopen("output.txt", "a+");
    int num;
    while (scanf(in,"%d", &num) !=EOF)
    {
        printf(out,"%d,", num);
    }
    fclose(in);
    fclose(out);
    return 0;
}
```    
(g)What is bit field?and how is it define?
<br>
Answer :       <br>
<p>
a bit field is a data structure that allows you to specify the size (in bits) of individual members within a structure. <br>

Bit fields are defined within a structure, and their declaration follows a specific syntax. Here's an example of how a bit field is defined:         <br>
</p>

```
struct BitFieldExample {
    unsigned int flag1 : 1;
    unsigned int flag2 : 3;
    unsigned int flag3 : 4;
};
```
*Here flag1, flag2, and flag3. Each bit field is declared using a colon (:) followed by the number of bits that the member should occupy.*
        
(h)  Write the output of the program.

```
Input:
asdedsjlk
```
```c
#include <stdio.h>

int main() {
    printf("Input:\n");
char s[20],p[20];
scanf("%[asd] %[^\n]",s,p);
printf("Output: s=%s p=%s\n",s,p);
    return 0;
}

```
Answer:

```
Input:
asdedsjlk
Output: s=asd p=edsjlk
 ```     

<div align="left">2. Answer the following Questions. (Any <b>Four</b>). &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4 &times; 5 = 20 </div>

(a) What is the p in the following statements?
<pre>
(I) int *p(char *a[]);
(II) int *p[10];
(III) int (*p)[10];
(IV)  int *p(void);
(V) int p(char *a);
</pre>
Answer:
<p>
(I) int *p(char *a[]); here p is a function that accept an argument which is an array of pointers to characters returns a pointer to an integer quantity.<br>
(II)int *p[10];  Here p is a 10-element array of pointers to integer quantities.<br>
(III) int (*p)[10];  Here p is a pointer to a 10-element integer array.      <br>
(IV) int *p(void);   Here p is a function that returns a pointer to an integer quantity.<br>
(V) int p(char *a); Here p is a function that accepts an argument which is a pointer to a character and returns an integer quantity.  <br>         </p>                   
(b)  Write the output of the program:

```c
#include<stdio.h>
int main(){
  int a=5,b=2,c=1;
  int *p=&a,*q=&b,*r=&c;
  *p+;b--;*r=*r+1;
printf("output1:a=%d b=%d c=%d\n",a,b,c);
*p=*q+++*r;*q=a+c;c=*r+*q;
printf("output2:a=%d b=%d c=%d\n",a,b,c);
c=(a++==b)?*p+2:*q--;
printf("output2:a=%d b=%d c=%d\n",a,b,c);
    return 0;
}
  ```
Answer:
```
output1:a=6 b=1 c=2
output2:a=5 b=1 c=7
output2:a=6 b=1 c=6
```              
(c)Write a program which will input an array of n sorted element.And input and search an element in the array by binary search.

Sample:
```
Input n= : 7
input n element:
1 2 3 4 5 6 6 
Enter a number which you search for: 
3
3 th number
```
Answer:
```c
#include<stdio.h>
int bsearch(int arr[],int n,int k){
    int fst=0,lst=n,cnt=0,mid;
    while(fst<=lst){
        mid=(fst+lst)/2;
        if(arr[mid]==k){
            return mid; 
        }
        else{
            if(arr[mid]<k){
                fst=mid+1;
            }
            else {
                lst=mid-1;
            }
        }
    }
    return -1;
}
int main(){
   int n,k,p;
   printf("Input n= : ");
   scanf("%d",&n);
   int arr[n];
   printf("input n element:\n");
   for(int i=0;i<n;i++){
       scanf("%d",&arr[i]);
   }
   printf("Enter a number which you search for: \n");
   scanf("%d",&k);
   p=bsearch(arr,n,k);
    if(p!=-1)printf("%d th number\n",p+1);
    else printf("Not Found\n");
    
    return 0;
}
```     
(d) 
 Given a single strand DNA code[n<1000].Find the compliment strand and Hydrogen bond in the genetic code by programming.[A=T,C triple bond G]
<br>
*Genetic CODE: AGCTACTGGTCACTAGACTG*

Answer:

```c
#include <stdio.h>
#include<string.h>

int main() {
    printf("write the genetic code: \n");
    char s[1000],Anti[1000];
    int Hn=0,n;
    scanf("%s",&s);
   

     for(int i=0;i<strlen(s);i++){
         if(s[i]=='A'||s[i]=='T'){
             Hn+=2;
             if(s[i]=='A')s[i]='T';
             else s[i]='A';
         }
         else{
             Hn+=3;
             if(s[i]=='G')s[i]='C';
             else if(s[i]=='C') s[i]='G';
             else {
                 printf("%c is not a genetic codon.\n",s[i]);
                 return 0;
             }
         }
     }
     printf("The compliment code is:\n %s\n",s);
     printf("Number of Hydrogen bond: %d\n",Hn);
     
     
     
    return 0;
}
```

```
write the genetic code: 
AGCTACTGGTCACTAGACTG
The compliment code is:
 TCGATGACCAGTGATCTGAC
Number of Hydrogen bond: 50
```

<div align="left">3. Answer the following Questions. (Any <b>Two</b>). &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2 &times; 10 = 20 </div>

(a)   
<p>Makha is very interested in Fibonacci number and storage class.His coding teacher Kulu wrote a code with recursion.But She is not interested in recursion.So,She asked you(as you are 2nd code teacher) to write code for fibonacci series without recursion but using storage class.Though,his brother interested in recursion, he could not find previous code.So,please write two code with recursion and without recursion.
</p>

Answer:
*Code for fibonacci series with recursion.*
```c
#include <stdio.h>

int fibonacci(int n)
{
     if(n==0)return 0;
     if(n==1)return 1;
    int f=fibonacci(n-1)+fibonacci(n-2);
    
    return f;
}

int main() {
    int n;
    printf("Input: \n");
    
    scanf("%d", &n);
    printf("Fibonacci Series: \n");
    
    for (int i = 0; i < n; i++) 
    {
        printf("%d ", fibonacci(i));
    }

    return 0;
}

```
*Code for fibonacci series without recursion but using static storage class:*
```c
#include <stdio.h>

int fibonacci(int n)
{
     if(n==0)return 0;
     if(n==1)return 1;
     static int f1=0,f2=1;
     int f=f1+f2;
     f1=f2;
     f2=f;
    return f;
}

int main() {
    int n;
    printf("Input: \n");
    
    scanf("%d", &n);
    printf("Fibonacci Series: \n");
    
    for (int i = 0; i < n; i++) 
    {
        printf("%d ", fibonacci(i));
    }

    return 0;
}
 ```      
(b)<p>Suppose,You are given the number of students in Your class is n[n<50] and their nick name.Their nick name separated and also end by comma.
You have to sort the string.so,write a program in c for sort these name and print with space.
</p>
Answer:
 
```c
#include<stdio.h>
#include<stdlib.h>
#include<string.h>
void sortstring(char s[][20],int n){

 for(int j=0;j<n;j++){
    for(int i=0;i<n-1;i++)
    {
        if(strcmp(s[i],s[i+1])>0)
        {
            char tem[20];
            strcpy(tem,s[i]);
            strcpy(s[i],s[i+1]);
            strcpy(s[i+1],tem);
        }
    }
 }
}

int main(){
  char s[50][20];
  int n;
  printf("Number of student:\n");
  scanf("%d",&n);
printf("Name of the student-saparated and end with comma:\n");
  for(int i=0;i<n;i++)
  {
    scanf("%[^,],",s[i]);
  }

  sortstring(s,n);
printf("Output:\n");
   for(int i=0;i<n;i++)
   {
     printf("%s ",s[i]);
   }

    return 0;
}
```
(c)<p>Generate all prime number less than 1000 using Sieve of Eratosthenes and print them in a triangular shape. Make sure that the shape must be same when printed 2 and 3 digit prime number.
Input will be n (the row number)[n<12].
</p>

```
INPUT:
2
Output: 
     2
  3  5  7

```

Answer:
```c
#include<stdio.h>
#define sz 1000
int num[sz],pr[1000];
int sieve(){
    int cnt=0;
    for(int i=3;i*i<=sz;i+=2)
    {
        for(int j=i*i;j<=sz;j+=i)
        {
            num[j]=1;
        }
    }
    
    for(int i=2;i<sz;i+=2){
         if(num[i]==0){
             
        pr[cnt]=i;
        cnt++;
        if(i==2)i--;
         }
        
       
    }
    
}

int main(){
    sieve();
    int n,cnt=0;
    printf("INPUT:\n");
    scanf("%d",&n);
      printf("Output: \n");
    for(int i=1;i<=n;i++)
    {
        for(int j=1;j<=n-i;j++)
        {
            printf("   ");
        }
        
        for(int j=1;j<=i;j++)
        {
            printf("%3d",pr[cnt]);
            cnt++;
        }
        for(int j=1;j<=i-1;j++)
        {
            printf("%3d",pr[cnt]);
            cnt++;
        }
        
        
        printf("\n");
    }
  return 0;  
}
```
*Sample :*
```
INPUT:
5
Output: 
              2
           3  5  7
       11 13 17 19 23
    29 31 37 41 43 47 53
 59 61 67 71 73 79 83 89 97
```
        


<div align="center">- End -</div>

- [x] I am declaring that, the above work is my own work. Whatever added above
except the template is the result of my brainstorming. I also understand that
submitting work that isn’t my own may result in permanent failure of this course
as well as the whole current semester.
