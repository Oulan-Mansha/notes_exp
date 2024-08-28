
- declaration ka waqt variable ka sath & lagna, ussa refrence variable bana deta hai.
- issa banata waqt initialize karna compulsory hai, sirf ordinary variables assign kar sakta hai.

![[Pasted image 20240720163916.png]]


```
int x = 5;
int *p;
p = &x; // yaha hum kaha ga x ka address y ma store kar raha hai. or ab y x ko                   point kara ga
int &y = x; // yaha hum kaha ga x ka refrence y ma store kar raha hai. or ab y x                 ko refer kara ga.
y++;   //agar humm ab y++ karaa ga tu wo x++ ho ga. jo ka pointer sa different                    hai,kio ka agar hum p++ karaa ga tu wo p++ ho ga. 

```
 - jab hum y ko access karaa ga tu matlab humm x ko access karaa ga, y sirf x ka dooosraa name hai.
 - hum ab y ko modify nahi kar sakta,matlab refrence variable aik dafa kissi variable ka refrence rakh la tu wo marta damm tak kissi doosra variable ka refrence apna andar store nahi kar sakta
 - jab ka pointer jab marzi kissi bhi variable ka address ya address ko point kar sakta hai.

![[Pasted image 20240720164610.png]]
![[Pasted image 20240720165043.png]]
