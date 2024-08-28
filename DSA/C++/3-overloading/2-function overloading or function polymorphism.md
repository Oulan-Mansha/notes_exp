
![[Pasted image 20240722163907.png]]

- **function declaration** -> return type, function name, function arguments.

![[Pasted image 20240722163700.png|100]]

- function is name is the most important thing, it is above function prototype.
- compiler function ka call ko daikh kar ya decide karta hai, kon si function defination bind(map, connect) ho gi. issi ko early binding kahta hai.

![[Pasted image 20240722164704.png]]

- jab program ban jata hai uss ka sath do kaam hi hota hai, aik compilation or doosra run. compilation, run sa pahla perform hota hai, or yaa kam compile time par hota hai, isss waja sa issaa **early** kahta hai
- or agar yaha kaam run_time par ho ga tu issa **late binding**  ya **dynamic binding**.
- function call ki function defination ka saath mapping hi binding kahlati hai.
- c ma compiler binding karna ka lia function ka name ko importance deta hai, agar c ka compiler function call ka lia, multiple defination daikha ga binding ka lia tu wo error da ga.

![[Pasted image 20240722170243.png]]


>[!tip]- function overloading
>when one function name overloaded with different jobs it is called function overloaded.(function polymorphism).

```
#include <iostream>

using namespace std;

int add(int,int);

int add(int,int,int);

int main()

{

int x,y,z;

cout<<"Enter two number : ";

cin>>x>>y;

cout<<"sum = "<<add(x,y)<<endl;

  

cout<<"Enter three numbers : ";

cin>>x>>y>>z;

cout<<"sum = "<<add(x,y,z)<<endl;

return 0;

}

  

int add(int a,int b)

{

return a+b;

}

  

int add(int a,int b,int c)

{

return a+b+c;

}
```

![[Pasted image 20240722173828.png]]

| C Compiler                                  | C++ compiler                                         |
| ------------------------------------------- | ---------------------------------------------------- |
| ya sirf name ko daikhta hai binding ka lia. | ya function signature ko daikhta hai binding ka lia. |


![[Pasted image 20240725144428.png]]

agar rule#1 ko use kar ka ya decide ho raha hai ka yahi candidate match ho raha hai, tu rule#2 and 3 par nahi jaye ga and soon.kissi bhi rule par agar decide ho jata hai, ka condidate match ho gaya hai tu agaa walaa rules ko check nahi kia jaye ga. agar teeno rules ko apply karna ka baad match nahi ho ga tu error aye ga.

- pahla rule tab fail hota hai jab arguments exactly match nahi hota hai.

>[!tip]- type conversion
>koi bhi primitive type kissi dosra primitive type ma convert ho sakta hai.
>
>![[Pasted image 20240725143349.png]]

| type conversion                | type promotion                             |
| ------------------------------ | --------------------------------- |
| iss ma data lo isss ma data loss nahi ho sakta.  i  i  i  i  i  i  i  i  i  |

3rd step type conversion ma argument saab data types ma convert ho ga, orr uss ka baad compiler function call ko function signature sa match karaa ga, jiss function signature sa match ho ga, uss ka saath binding kar da ga. 

![[Pasted image 20240725144028.png]]

agar multiple function signatures sa match ho jaye tu **"ambiguity error "** aye ga.