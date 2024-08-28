

## Arithmetic Instructions : 

- any line/instruction who manipulate data with the help of operator(s).
-  3 + 4

## Classification of Operators
###  1-unary operator
- It requires only one operand

>[!abstract]+ Types
> > [!info]-  unary_plus (+) , unary_minus(-)
> > they will tell the type of the number (positive or negative).
> > +5 , -7
> 
> > [!info]- increment operator(++)
> > it will increase the value by 1 of variable.
> > 
> > >[!types]-  Types
> > >>[!note]+ note
> > >post increment and post decrement both has same priority
> > >>>[!info]- post_increment
> > >   it has least priority, if one expression contains more than one operator(any type) than it will execute after the execution of all expression operators.
> > >  >>[!code] example
> > >  >> #include <stdio.h> 
> > >  >> int main() 
> > >  >> {
> > >  >>  int num1 = 5;
> > >  >>   int num2;
> > >  >>    // Example of post-increment operator 
> > >  >>    num2 = num1++; 
> > >  >>    // Output the results
> > >  >>     printf("num1 = %d\n", num1); 
> > >  >>     // Output: num1 = 6 (num1 is incremented after assignment) 
> > >  >>     printf("num2 = %d\n", num2); 
> > >  >>     // Output: num2 = 5 (num2 gets the value before increment) 
> > >  >>     return 0; }
> > >  >>     
> > >  >
> > >> > [!info]- pre_increment
> > >  >> it has highest priority, if one expression contains more than one operator(any type) than it will execute before the execution of all expression operators.
> > >  >> >[!code] example
> > >  >> >#include <stdio.h> i
> > >  >> >nt main()
> > >  >> > { int num1 = 5;
> > >  >> >  int num2; 
> > >  >> >  // Example of pre-increment operator
> > >  >> >   num2 = ++num1;
> > >  >> >    // Output the results 
> > >  >> >    printf("num1 = %d\n", num1); 
> > >  >> >    // Output: num1 = 6 (num1 is incremented before assignment)
> > >  >> >     printf("num2 = %d\n", num2); /
> > >  >> >     / Output: num2 = 6 (num2 gets the incremented value) 
> > >  >> >     return 0; }
> > >  >> >
> 
> >[!info]- decrement operator(--)
> > it will decrease the value by 1 of variable.
> > >[!code]- decrement - example
> > >#include<stdio.h>
> > >int main()
> > >{
> > >	int x = 5;
> > >	x--; // x = x - 1;
> > >}
> 
> > [!info]- sizeof()   operator
> > in the parenthesis of it we can either write :
> > 1- data type 
> > 2- variable
> > 3- constant
> > it tells the size in bytes of that thing which is in its parenthesis
> > >[!code]- example
> > > ------------- Data Type --------
> > > int x;
> > > x = sizeof(float);
> > > printf("%d",x); // 4
> > > 
> > > x = sizeof(double);
> > > printf("%d",x); // 8
> > > 
> > > x = sizeof(char);
> > > printf("%d",x); // 1
> > > 
> > > ---------- variable ---------
> > > 
> > > int x,y;
> > > char m;
> > > double d1;
> > > x = sizeof(d1); // 8
> > > x= sizeof(m); // 1
> > > x= sizeof(int); // 4
> > > 
> > > --------- constant ---------
> > > 
> > > x = sizeof(35) // 4 -> integer constant is int type
> > > x = sizeof(4.7) // 8 -> real constants are by default of double type
> > > x = sizeof('a') // 4 -> here character constant will be replaced by ascii and ascii is integer value which means it take 4 bytes in memory. 



### 2- arithmetic operators ([[arithmetic operators]])

### 3- bitwise operators ([[bitwise operators]])

### 4- relational operators ([[relational operators(comparison operators)]])

### 5- logical operators ([[logical operators]])

### 6- Assignment operators



![[assingment.png]]

### 7- Compound Assignment operator


>[!tip]- Compound Assignment 
> - they are made from two operators.
> - they treated as a single operator, but their working is = two operators



![[Pasted image 20240622114945.png]]


