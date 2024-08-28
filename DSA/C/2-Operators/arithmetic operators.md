
## * / %  
###### they have the same priority (but higher than +,-) and if they come in same expression then expression will be evaluate from left to right.

## + -

###### they have the same priority (but less than * / %) and if they come in same expression then expression will be evaluate from left to right.

```
#include <stdio.h>

int main()
{
	a * b / y; // here expression will be evaluated from left to right
	a + b * y; // in this expression * will be evaluated first then addition will be evalvated
}
```





>[!info] imp info about /
>- if we divide integer by integer than we will get integer as a result. 1/2 = 0
>- if we divide integer by real (vice versa) and real by real then will get real. 
>     	3 / 4.0 = 0.75
>     	 3.0 / 4  = 0.75
>     	 3.0 / 4.0 = 0.75 	
> 
> - if we divide a number(x) by 10 then we will get that number without last number.
>       25/10 = 2 


 >[!imp] imp info about %
 >
 > - if we take mode of a number (x) by 10 then we will get a last number of that number.
 >25 % 10 = 5
 > - if we get x % (any number(y)) == 0 , then we are 100% sure that  y completely divides x
 >but in case of x / y  we are not 100 % sure because 15/3 , 16 / 3 and 17 / 3 has the same answer = 5
 > -  if we take mode of smaller number with larger number then we will get the smaller number. 3 % 4 == 3.
 > - we cannot apply modulus operator on real numbers, it will cause an error
 


## return ([[1-types of operators]])