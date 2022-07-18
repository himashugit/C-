# First Programm

```c++
#include <iostream>   //this is the library, contains built in func,prog.
using namespace std;  // built in lib contain under std namespace0.02  
 
int main() //main function,int here is return type func
{

  cout<<"hello world"; // console out, this is to prin msg on screen << (insertion operator)

  return 0; //funrction return here

}
```
# How to write a prog for adding 2 number

- Input - print "Enter 2 number" a,b;
- process - c=a+b
- output = print "Addition is, " c;

In C you will do like this

```c++
 #include <iostream>
 using namespace std;

 int main()
 {
     int a,b,c
     cout<<"Enter 2 no";
     cin>>a>>b;
     c=a+b;
     cout<<"addition is"<<c;
     return 0;

 }

```
```c++
#include<iostream>
using namespace std;

int main()
{
    string name;
    cout<<"May I know your name ";
    getline(cin,name); // to accomodate multiple strings in name
    cout<<"Welcome Mr "<<name;
    return 0;
}

```

# Data Types




# precedence and expression


| **operator**    | Assumed precedence                         |
| ------------------------ | ----------------------------------- |
| **()**   | 3 |
| **(*), /, %**   | 2 |
| **+-**    | 1 |

- Area of a triangle a=1/2bh

a= b*h/2

a=0.5*(b*h)

- Perimeter of rectangle P=2*(l+b)
- sum of n terms S=n*(n+1)/2
- terms of A.P series t=a+(n-1)*d
- root of quadratic Ex r=(-b+sqrt(b*b-4*a*c))/(2*a)
-Speed S=(v*v)-(u*u)/(2*a);

S=pow(v,2)-pow(u,2)/(2*a);

# Program for Area of Triangle

Area=(b*h)/2

- Input
- Process
- Output



```c++
#include <iostream>
using namespace std;
int main()

{
    float b,h,a;
    cout<<"Enter base & height";
    cin>>b>>h;
    a=(b*h)/2;
    cout<<"Area is" <<a;

}

```

# Finding sum of n natural num

```c++
#include <iostream>
using namespace std;
int main()
{
    int n, sum;
    cout<<"Enter n";
    cin>>n;
    sum=n*(n+1)/2;
    cout<<"sum is"<<sum;

}
```

# Finding Roots of a Quadratic equation
ax2+bx+c=0


| **Start**    | will start prog here                         |
| ------------------------ | ----------------------------------- |
| **Print 'Enter a,b,c'**   | this will read a,b,c |
| r1=(-b+sqrt(b*b-4*a*c))/(2*a)  | this is how we will write in c++ |
| **print the resul**    | "Roots are", r1,r2; |
| **Stop**    | 

- sqrt equation
```c++
#include <iostream>
#include <math.h>
using namespace std;
int main()
{
    float a,b,c,r1,r2;
    cout<<"Enter a,b,c";
    cin>>a>>b>>c;
    r1=(-b+sqrt(b*b-4*a*c))/(2*a)
    r2=(-b-sqrt(b*b-4*a*c))/(2*a)
    cout<<"roots are"<<r1<<""<<r2;
    return0;
}
```

- calculate speed 
```c++
#include <math.h>
#include<iostream>
using namespace std;

int main()
{

  int u,v,a;
  float speed;
  
  cout<<"Enter 3 number";
  cin>>u>>v>>a;
  speed=(u*u-v*v)/(2*a);
  cout<<"spped is"<<speed<<endl;
  return 0;
  
}
```
Calculate Distance- write an expression for calculating distance

```c++
#include<iostream>
int CalculateDistance(int u, int v, int a)
{
    float distance;
    distance=(v*V-u*u)/(2*a)
    return distance;
}
```
Calculate SI
P - Principle amount
R - Rate of Interest
T - Time

```c++
int SimpleInterest(int P,int T, int R)
{
    float SI;
    SI=P*R*T/100.0;
    return SI;
}
```

Calculate Vol of a cylinder
3.14*r*r*h

```c++
float CylinderVolume(int radius, int height)
{
    float volume;
    volume=3.14*radius*radius*height;
    return volume;
}
```
Calculate distance b/w 2 point
x1,y1 = first point
x2,y2 = Second point

```c++
#include<cmath>
float distance(int x1, int y1, int x2, int y2)
{
    float dist;
    dist=sqrt(x2-x1)*(x2-x1)+(y2-y1)*(y2-y1);
    return dist;
}
```

Compoud assignment
```c++
#include <iostream>
using namespace std;
int main()
{
    int sum=10;
    int x=5;
   // sum=sum+x;
    sum+=x;
    sum*=x;
    cout<<sum;
    return 0;
}
```

PreIncrement & Post Increment

```c++
int x=5 , y=10, z;
z = ++x*y;
z=6*10
z=60


z=x++*y;
z=50
x=6
```

```c++
#include <iostream>
using namespace std;
int main()
{
    i=5;
    i++;
    cout<<i <<endl;
    retrun 0;
}
```

# Overflow
Range of  char -128 to 127

-  Char has 1byte. 1byte has 8bits (0-7)
- 1Byte can store 0-255 char
- 0 being least significant, 7 is most
- 127 binary would be
- 01111111
- here 0 at start it means it is positive, if 1 -ve

Data has 2 types

- Number
- Char/ALphabetic

- Primitive Data Type
    - Integral
        - int
        - Char

    - bool

    - Floating pont
        - float
        - double

 - userdefined
    - enum
    - structure
    - union
    - class

- Derived
    - Array
    - Pointer
    - Reference


|Data Types | Size | Range 
| --- | --- | --- | 
|int|2 or 4|-32768 to 32767
|float|4|-3.4*10^-38 to 3.4*10^38
|double|8|-1.7*10^-308 to 1.7*10^308
|char|1|-128 to 127
|bool|undefined|true/false

- How int has 32768 value

ex - lets take 2 byte

`15 14 13 12 11 10 9 8 7 6 5 4 3 2 1 0`

15 is the most signiificant bit. If this bit is 0, it is positive
if it is 1 then its negative

0 least significant bit.

`2^15 = 32768`

char has ASCII 

`A - 65`

`B - 66`

`z - 90`

`a - 97`

`b - 98`

`c - 122`

`0 - 48`

`1 - 49`

`9 -57`

Modifier

- unsigned - 0-65535 (unsigned int)

    unsigned char 0-255

- long - long int 4bytes, 8 bytes

- long double - 10byte


# Variables 

where we store data.

```c++
    int main()
    {
        int rollno = 25;
        //rollno = 25;
        char group = 'A'; //char should be single quote
        float price = 15.21f; // f to tell it is float, if not defined it will take as double.


    }

```

# operators & Expressions

 - Airthmetic - +, -, *, ./.
 - Relational - <, >, <=, >=, ==
 - Logical - &&, ||, !
 - Bitwise - &, |, ~, ^
 - Increment/Decrement - ++, --
 - Assignment - =


 ```c++
    int main()
    {
        int a,b,c;
        a=5
        b=6
        c=a+b
        cout<<c;<<endl;
        return 0;
    }
 ```

```c++
#include<iostream>
using namespace std;

int maint()
{
    char x=127;
    x++;
    cout<<(int)x;<<endl;
    return 0;

}
```
- This expression give you int max value
```c++
#include<iostream>
#include<climits>
using namespace std;

int main()0.0172
{
    int x=INT_MAX;
    x++;
    cout<<(int)x<<endl;
    return 0;

}
```
# BitWise Operator

 **&**    | and                 |
| ------------------------ | ----------------------------------- |
| **!**   | or |
| **^**   | xor |
|**~**   | nor |
|**<<**  | left shit|
|**>>**  | right shift|

|bit1 | bit2 | bit1 & bit2 |
| --- | --- | --- |
| 0 | 0 | 0
|0|1|0
1|0|0
1|1|1


|bit1 | bit2 | bit1 xor bit2 
| --- | --- | --- | 
|0|0|0
|1|1|1
|1|0|1
|0|1|1

int x=11, y=5;

x =       00001011

y = 00000101

128 64 32 16 8 4 2 1

int x = 5, y;

x=    00000101

x<<1         000001010 - one bit shif to left here

formula is x>>i   x=2*i

so here x is 10

for right shift formula is x/2i

so x = 5/2 = 2

```c++
#include <iostream>

using namespace std;

int main()
{
    int x =5, y =7, z;
    z = x&y;
    \\z = x | y;
    cout<<"value of z is " <<z<<endl;
    return 0;
}
```

```c++
#include <iostream>

using namespace std;

int main()
{
    char x =5, y ;
    y = x<<1;
    cout<<"value of y is " <<(int)y<<endl;
    
}
```

# Enum and Typedef



|  Depart |  Menu |  Days | Card Colors  | Feedback  |
|---|---|---|---|---|
|CS|File|Mon|club|poor
|ECE|New|Tue|Spade|satisfactory
|IT|Open|Wed|Diamond|good
|Civil|save|Thur|Hearts|good

- we can define them using 2 method here
- const int cs =1

const int ECE =2

const int IT =3

OR

enum day{mon,tue,wed,thur,fri,sat,sun};

- days is here user defined data type and we can use it as

```c++
int main()
{
    day d; // day is data type(userdefine) and d is var
    d =mon;
    d = fri;
    d = 0;// you can not use it like this
}
```

```c++
enum depart(cse=1,ece,it,civil)//assigned cse=1 else it will start from 0

int main()
{
    depart d;
    d=cse;

}
```

# typedef
```c++

int main()
{
    int m1,m2,m3,r1,r2;
}
```
This way of wrting a code is not a good practice as var m1,m2--- are not depicting what are they.

So in order to define the correct type for readability we can use them as

```c++
typedef int marks;
typedef int rollno;

int main()

{
    marks m1,m2,m3;
    rollno r1,r2;
}

```

```c++
#include <iostream>

using namespace std;

enum day {mon,tue,wed,thur,fri,sat,sun};

int main()
{
    day d;
    d =tue;
    cout<<"value of day is " <<d<<endl;
    
}

```

```c++

#include <iostream>

using namespace std;

enum day {mon=1,tue,wed,thur=10,fri,sat,sun};

int main()
{
    day d;
    d =tue;
    cout<<"value of day is " <<d<<endl;
    cout<<"value of day is " <<tue<<endl;
    cout<<"value of day is " <<thur<<endl;
    cout<<"value of day is " <<fri<<endl;
    cout<<"value of day is " <<sat<<endl;
    cout<<"value of day is " <<sun<<endl;
       
}

Result

value of day is 2
value of day is 2
value of day is 10
value of day is 11
value of day is 12
value of day is 13

```

# Data Type

A program has data and set of instructions to perform on it. A program has the below set

- Code section - instructions
- Stack - contains data i.e variable
- Heap
 - Main memory



Data has 2 types

- Number
- Char/ALphabetic



# Conditional Statement :-

- Relational operator

> <, > <=, >=, !=, ==



 - Find max of 2 numbers

```c++
    #include <iostream>
    using namespace std;

    int main()
    {
        int a = 5;
        int b = 4;
        if (a<b)
        {
           cout<<"a is greater than b"<<endl;
        }
                
        else{
            cout<<"b is greater than a"<<endl;
        }
        
        return 0;
        
    }
```
```c++
#include <iostream>
using namespace std;

int main()
{
    int roll;
    cout<<"Enter your rollno";
    cin>>roll;

    if (roll<10)
    {
        cout<<"rollno is invalid";

    }
    else{
        cout<<"rollno is valid";
    }
    return 0;
    }
```

- Number odd /even

```c++

#include <iostream>
using namespace std;

int main()

{
    int num;
    cout<<"Enter an integer: ";
    cin>>num;
    
    if(num%2==0)
    
      cout<<num <<" is even"<<endl;
    
    else
      cout<<"odd"<<endl;
      
    return 0;
}
```
```c++

#include <iosteam>
using namespace std;

int main ()

{
    int a,b,c;
    cout<<"enter 2 number: ";
    cin>>a>>b;
    if (b==0)
      cout<<"division by zero"<<endl;
    else
    {
        c=a/b;
        cout<<c<<endl;

    return 0;

    }
}

```

# Logical Operators

 - && and
- || OR
- ! Not


> AND output

|bit1 | bit2 | bit1 & bit2 |
| --- | --- | --- |
|T|T|T
|T|F|F
|F|T|F
|F|F|F

> OR Output


|bit1 | bit2 | bit1 & bit2 |
| --- | --- | --- |
|T|T|T
|T|F|T
|F|T|T
|F|F|F

> Not Output

|bit1 | bit2 
| --- | --- 
|T|F
|F|T


- Compound condition 

```c++
#include <iostream>
using namespace std;

int main ()

{
    int hrs;
    cout<<"enter time: ";
    cin>>hrs;
    if (hrs>=9 && hrs<=18)
      cout<<"working"<<endl;
    else
    {
        cout<<"leisure time"<<endl;

    return 0;

    }
}
```

OR Operator use case for offer

```c++

#include <iostream>
using namespace std;

int main()

{
    int age;
    cout<<"Enter your age ";
    cin>>age;
    
    if (age<12 || age>55)
        cout<<"You're eligible"<<endl;
    
    else
        cout<<"You're not eligible"<<endl;
    
    return 0;
    
}

```

Nested If condition

```c++
#include <iostream>
using namespace std;

int main()

{
    int a,b,c;
    cout<<"Enter 3 no. ";
    cin>>a>>b>>c;
    
    if(a>b && a>c)
        cout<<a;
    else if(b>c)
        cout<<b;
    else    
        cout<<c;
        
    return 0;
    
}
```

Nature of root

- Quadratic equation

> ax2+bx+c=0

roots = -b+-root(b*b-4*a*c)/(2*a)

discriminant 

> d=b2-4ac

if d=0 , real & qual

if d>0 , real & unequal

if d<0 , imaginary

```c++
#include <iostream>
using namespace std;
#include<cmath>

int main()
{
    int a,b,c,d,r1,r2;

    cout<<"Enter a,b & c";
    cin>>a>>b>>c;
    d = b*b-4*a*c;

    if (d==0)
    {
       cout<<"roots are real & equal";
       cout<<endl<<(-b/(2*a)); 
    }
        

    else if (d>0)
    {
        cout<<"roots are real & unequal";
        cout<<endl<<(-b+sqrt(d))/(2*a);
        cout<<endl<<(-b-sqrt(d))/(2*a);
    }
    else
    {
        cout<<"imaginary";
    }

    return 0;
}
```

Conditional stat for Grades 

```c++
#include <iostream>
using namespace std;
#include<cmath>

int main()
{
    int m1,m2,m3, total;
    float Avg;

    cout<<"Enter marks of 3 subj: ";
    cin>>m1>>m2>>m3;
    total = m1+m2+m3;
    Avg = total/3.0;
    
    if (Avg>=60)
        cout<<"good marks";
    else if (Avg>=35 && Avg<60)
        cout<<"medium";
    else
        cout<<"poor";

    return 0;
}
```

else if ladder

```c++
#include <iostream>
using namespace std;
#include<cmath>

int main()

{
    int day;
    std::cout << "Enter day number" << std::endl;
    cin>>day;
    
    if (day == 1)
    {
        cout<<"Monday";
    }
    else if (day == 2)
    {
        cout<<"Tue";
    }
    else if (day == 3)
    {
        cout<<"Wed";
    }
    else if (day == 4)
    {
        cout <<"Thus";
    }
    else if (day == 5)
        
        cout <<"Fri";
    else if (day == 6)
    {
        cout <<"Sat";
    }
    else if (day == 7)
    {
        cout <<"Sun";
    }
    else
    {
        cout <<"Invalid number";
    }
    
    return 0;
}
```

# Short Circuit

> if (a>b && b>c)

if a>b = True then it will  check for other conditon and result is true

if a>b = false then it'll not check for second condition

> if (a>b || b>c)

if first it True then it'll not check for second 

```c++

#include <iostream>
using namespace std;
#include<cmath>

int main()

{
    int a=5, b=3, i=7;
    
    if (a>b || ++i<=b)
    {
        
    }
    cout<<i<<endl;
    
    return 0;
}

```
# Dynamic Declaration 

You can assign var within the code statement, rather defining all the var in main.

```c++
#include <iostream>

using namespace std;

int main()
{
    int a,b,c;
    
    if (a>b)
    int z //insteam of defining var in the main, we defined this in the if condition. Using this way we save some memory and make prog fast processing.
}
```

```c++
#include <iostream>

using namespace std;

int main()
{
    int a,b,c;
    
    if (int k=exp; k<a>)// you can defined this way as well.

}
```

```c++
#include <iostream>

using namespace std;

int main()
{
    int a=5,b=7;
    {
    int c=a+b;
    if (c>10)
    {
    cout<<c<<endl;
    }
    
    }
}
```

```c++
#include <iostream>

using namespace std;

int main()
{
    int a=5,b=7;
    {
    
    if (int c=a+b;c>10) //you can use it in c++ 17
    {
    cout<<c<<endl;
    }
    
    }
}
```

# Switch Case

```c++
#include <iostream>

using namespace std;

int main()
{
    int day;
    cout<<"Enter the day no: ";
    cin>>day;
    switch(day)
    {
        case 1: cout<<"Mon";
            break;
            
        case 2: cout<<"Tue";
            break;
            
        case 3: cout<<"Wed";
            break;
            
        case 4: cout<<"Thu";
            break;
            
        case 5: cout<<"Fri";
            break;
            
        case 6: cout<<"Sat";
        
        case 7: cout<<"Sunday";
            break;
            
        default: cout<<"Invalid number";
        
        
    }
}
```

- Switch case ex
```c++
#include <iostream>

using namespace std;

int main()
{
   int option;
   cout<<"Menu\n";
   cout<<"1. add\n"<<"2. sub\n"<<"3. multi\n"<<"4. div\n";
   cout<<"Enter your choice ?- ";
   cin>>option;
   int a,b,c;
   cout<<"Enter 2 number: ";
   cin>>a>>b;
   
   switch(option)
   {
       case 1: c=a+b;
            break;
        
        case 2: c=a-b;
            break;
        case 3: c=a*b;
            break;
        case 4: c=a*b;
            break;
        
   }
   cout<<"result is "<<c<<endl;
   return 0;
}
```

- Switch case example for airthmatic ops

```c++
#include <iostream>

using namespace std;

int main()
{
   int x,y,z,choice;
   cout<<"Enter your choices 1,2,3,4 ?\n";
   cin>>choice;
   cout<<"1. add 2 no\n"<<"2. sub 2 no\n"<<"3. multi 2 no\n"<<"4. div 2 no\n";
   cout<<"Any 2 number ?";
   
   cin>>x>>y;
   
   switch(choice)
   {
       case 1: z=x+y;
       break;
       case 2: z=x-y;
       break;
       case 3: z=x*y;
       break;
       case 4: z=x/y;
       break;
       
       default: cout<<"invalid choice\n";
       break;
   }
   
   cout<<"result is "<<z<<endl;
   
   return 0;
}
```

- bill payment using if-elseif
```c++
#include <iostream>

using namespace std;

int main()
{
    float billamount;
    float discount = 0.0;
    cout<<"what is the billamount? : ";
    cin>>billamount;
    
    if (billamount>=5000)
        discount=billamount*20/100;
    else if (billamount>2000 && billamount <5000)
        discount=billamount*10/100;
    else
        cout<<"No discount, sorry :( \n" ;
        
    cout<<"your Bill is : "<<billamount<<endl;
    cout<<"Your discount is : " <<discount<<endl;
    cout<<"to be paid : "<<billamount-discount<<endl;
    
   
   return 0;
}
```
 # Conditions & Loops

 While

 ```c++
#include <iostream>
using namespace std;

int main()
{
    int n,i=1;
    cout<<"Enter value of n ";
    cin>>n;
    while(i<=n)
    {
        cout<<i<<endl;
        i++;
    }
    
 return 0;
}

 ```

 Do - First process and then check condition

 ```c++
#include <iostream>
using namespace std;

int main()
{
    int n,i=1;
    cout<<"Enter value of n ";
    cin>>n;
    do
    {
        cout<<i<<endl;
        i++;
    } while(i<=n);
    
 return 0;
}

 ```

 For Loop check
 ```c++
#include <iostream>
using namespace std;

int main()
{
    int n,i=1;
    cout<<"Enter value of n ";
    cin>>n;
    for (i=1;i<=n;i++)
    {
        cout<<i<<endl;
    }
    
 return 0;
}
 ```

 Multiplication Table using for loop

 ```c++
 #include <iostream>
using namespace std;

int main()
{
    int n,i;
    cout<<"Enter value of n ";
    cin>>n;
    for (i=1;i<=10;i++)
    {
        cout<<n<<"x"<<i<<"="<<i*n<<endl;
        
    }
    
 return 0;
}
```

```c++
#include <iostream>
using namespace std;

int main()
{
    int n,i,sum=0;
    cout<<"Enter value of n ";
    cin>>n;
    for (i=1;i<=n;i++)
    {
        sum+=i;
        
    }
    cout<<"sum on n no is "<<sum;
    
 return 0;
}
```

Factorial of n 

n! = 1*2*3*4*5*6 = 720

```c++
#include <iostream>
using namespace std;

int main()
{
    int n,i,fact=1;
    cout<<"Enter value of n ";
    cin>>n;
    for (i=1;i<=n;i++)
    {
        fact*=i;
        
    }
    cout<<"factorial of no "<<n <<"is" <<fact;
    
 return 0;
}
```
Factors of a no

IF number n%i==0 it is a factor.

let's take a number n==8 and if we divide this by 1,2,3,4,5,6,7,8.

```c++
#include <iostream>
using namespace std;

int main()
{
    int n,i;
    cout<<"Enter value of n ";
    cin>>n;
    for (i=1;i<=n;i++)
    {
        if(n%i==0)
        {
            cout<<i<<endl;
        }
        
    }
    
    
 return 0;
}
```
 -Perfect number

 ```c++
 #include <iostream>
using namespace std;

int main()
{
    int n,i,sum=0;
    cout<<"Enter value of n ";
    cin>>n;
    for (i=1;i<=n;i++)
    {
        if(n%i==0)
        {
            sum+=i;
        }
        
    }
    if(2*n==sum)
        cout<<"Perfect number";
    else
        cout<<"Not a Perfect number";
    
    
 return 0;
}
```

- Prime Number
```c++

#include <iostream>
using namespace std;

int main()

{
    int i,n,count=0;
    cout<<"Enter the number";
    cin>>n;
    
    for(i=1;i<=n;i++)
    {
        if(n%i==0)
        {
            count++;
        }
    }
    if(count==2)
    cout<<"prime number";
    else
    cout<<"Not a prime number";
    
    return 0;
}
```
- Counting Table
```c++
#include <iostream>
using namespace std;

int main()

{
    int i,n;
    cout<<"Enter the number ";
    cin>>n;
    
    for(i=1;i<=10;i++)
    {
        cout<<n<<"X"<<i<<"="<<n*i<<endl;
    }
    
    
    return 0;
}
```
- Natural number sum
```c++

#include <iostream>
using namespace std;

int main()

{
    int i,n,sum=0;
    cout<<"Enter the number ";
    cin>>n;
    
    for(i=1;i<=n;i++)
    {
        sum+=i;
    }
    cout<<"Sum of first " <<n<<" Natural number is "<<sum<<endl;
    
    return 0;
}
```
Display digit of a number 1724

we need to display it as 4 3 7 1. So first we need to take a number and then modeby(%)10. then the remainder would be that number. so if you mode 1724 by 10 remainder will be 4. Now to make the number ending with 2, we need to divide the number 10 and keep on doing this untill it is 0.

```c++
#include <iostream>
using namespace std;

int main()

{
    int n,r;
    cout<<"Enter a number";
    cin>>n;
    while(n>0)
    {
        r=n%10;
        n=n/10;
        cout<<r<<endl;
    }
    
    return 0;
}
```

- Armstrong Number calculation - A number added with their quebic equation is termed as Armstrong number. So if their addition comes as the number itself then that is known a armstrong number

ex 123 = 1+8+27=36 - not a armstron nu
153 = 1+125+27=153 - armstrong number

```c++
#include <iostream>
using namespace std;

int main()

{
    int n,r,sum=0,m;
    cout<<"Enter a number ";
    cin>>n;
    m=n;
    while(n>0)
    {
        r=n%10;
        n=n/10;
        sum=sum+r*r*r;
    }
    if(sum==m)
    cout<<"Number is armstrong";
    else
    cout<<"Number is not armstrong";
    
    return 0;
}
```

- Reversing a numnber - Procedure will remain same to get the each digit separately for a number. here we'll take a var as rev==0, rev=rev*10+r, this will give the reverse number.

```c++
#include <iostream>
using namespace std;

int main()

{
    int r,n,rev=0;
    cout<<"Enter a number ";
    cin>>n;
    
    while(n>0)
    {
        r=n%10;
        n=n/10;
        rev=rev*10+r;
        
    }
    
    cout<<rev<<endl;
    
    return 0;
}
```



- GCD of 2 numbers
```c++
#include <iostream>
using namespace std;

int main()

{
    int m,n;
    cout<<"Enter 2 number ";
    cin>>m>>n;
    
    while(m!=n)
    {
        if(m>n)
        m=m-n;
        else
        n=n-m;
        
    }
    
    cout<<m<<endl<<n;
    
    return 0;
}
```
# Arrays

- We can define list of array like this


`int A=[10] {1,2,3,4,5,6,7,8,9,0}`

 - How to print the list of arrays

 ```c++
 #include <iostream>
using namespace std;

int main()

{
   int A[5]={2,3,5,7,9};
   int i=0;
   for(i=0;i<5;i++)
   {
     cout<<A[i]<<endl;  
   }
   
    
    return 0;
}
```

- We can have int,float,char type of array

`int A[5]={1,2,4,5,6};`

`float B[5]={1.1,1.2,1.3,1.4,1.5};`

`char C[5]={'A','B','C','D','E'};`

`int A[4]={1,2};` - Remaining will be zeros

`int B[]={1,2,4,6};` - You can initialize like this as well.

```c++

#include <iostream>
using namespace std;

int main()

{
   char A[5]={65,'B',68,77,'C'};
   
   for(char x:A)// You can use this auto assign array feture.
   {
     cout<<x<<endl;  
   }
   
    
    return 0;
}
```
- Foreach loop

```c++
#include <iostream>
using namespace std;

int main()

{
   char A[5]={65,'B',68,77,'C'};
   
   for(char x:A)// You can use this array feture for_each type.you don't need to mention the size here it will iterate itself to the desire no.
   {
     cout<<x<<endl;  
   }
   
    
    return 0;
}
```
```c++
#include <iostream>
using namespace std;

int main()

{
   int A[5]={65,'c',68,77,3};
   
   for(auto x:A)// auto feature use to check the data type and use it to get the result, 
   {
     cout<<x<<endl;  
   }
   
    
    return 0;
}
```
- Sum of Array

```c++
#include <iostream>
using namespace std;

int main()

{
   int A[]={2,4,6,8,10,12};
   int n=6, sum=0;
   
   for(int i=0;i<6;i++)//for loop to get the i as count.
   {
     sum+=A[i];
   }
   cout<<"sum is "<< sum;
    
   return 0;
}
```
- Sum of Array Elements
A={4,8,6,9,5,2,7}

max=0;

|i | A[i] | if A[i]>max;max=A[i] |
| --- | --- | --- |
|0|4|4
|1|8|8
|2|6|8
|3|9|9
|4|5|9
|5|2|9
|6|7|9

```c++
#include <iostream>
using namespace std;

int main()

{
   int A[7]={4,8,6,9,5,2,7},
   n=7,max;
   max=A[0];
    
   for(int i=1;i<7;i++)
   {
       if (A[i]>max)
       {
           max=A[i];
       }
   }
   cout<<"Max element is "<<max;
   return 0;
}
```

- Binary Search

A={6,8,13,17,20,24,25,23,33,43}

0 l->>>>>>>>9 h

key=25

|l | h | mid(l+h)/2 |
| --- | --- | --- |
|0|9|0+9/2=4
|5|9|5+9/2=7
|5|6|5+6/2=5
|6|6|6+6/2=6

```c++
#include <iostream>
using namespace std;

int main()
{
    int A[10]={6,8,13,17,20,22,25,28,30,35};

    int l=0, h=9, key,mid;

    cout<<"Enter Key";
    cin>>key;
    while(l<=h)
    {

        mid=(l+h)/2;
        if(key==A[mid])
        {
            cout<<"Found at"<<mid;
            return 0;
        }
        else if(key<A[mid]) h=mid-l;
        else l=mid+l;
}
cout<<"Not found";

return 0;
}
```
O(n) - Linear search
O(log n) - Binary search is faster.

- Count number of +ve & -ve
```c++
#include <iostream>
using namespace std;

int main()
{
    int A[]={3,5,-2,9,-4,-10,-24,19,18,-7,8};
    int pcount=0;
    int ncount=0;
    
    for(int x:A)
    {
        if(x<0)
            ncount++;
        else
            pcount++;
    }
    cout<<"-ve count "<< ncount<<" "<<"+ve count "<<pcount;

return 0;
}
```




