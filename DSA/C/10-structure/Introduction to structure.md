


![[Pasted image 20240718055522.png]]


# primitive data type

ya aissa data types hai jin ki madad sa jab hum koi variable banata hai usss ma aik hi value store karwa sakta hai.
in ko pre-define data type bhi kahta hai.
in ka matlab compiler ma already define hai.

# non-primitive data type

opposite of primitive data type.
ya primitive data type sa mil kar banta hai.


![[Pasted image 20240718061948.png]]

![[Pasted image 20240718062053.png]]

jab hum real world ma kaaam kar raha ho ga, or humaa aik library managment system bana paraa, usss ma aik book ka data store karana paraa ga tu hammaa buhat zayada variables banana paraa ga. or isssi tarha student jisse book issue ki hai. agar humm na aissaa 1000 books or students ka record rakhna paraa ga tu baraa program ma buhat mushkil paish aye gi, jab unn variables ko function ma pass karaa ga tab bhi buhat parashani ho gi.

inhi problems sa pachna ka liya hum, aik book(non-primitive data type) bana la ga. jiss sa humm aik variable sa book ki information ko handle kar paye ga.


# defining structure

![[Pasted image 20240718100946.png]]

>[! tip]- imp
>- jab humm structure ko kisi function ka andar define karaa ga tu hummm usss data type ka variable sirf ussi function ka andar bana saka ga. or agar globally define karaa ga tu ussssa pura function ka andar istaamaal kar saka ga.
>	- jab hum structure ko define karaa ga tu wo koi memory consume nahi karaa ga.kio ka hum aik data type bana raha hai.or data type koi memory consume nahi karti. laikin agar data type (primitive ya non-primitive) sa koi variable banaye ga tu, wo variable memory consume karaa ga.
# declaring structure variable

![[Pasted image 20240718114813.png]]

>[!tip]- struct keyword
>C language ka aik rule hai ka jabb bhi hummm struct data type ka koi variable banataa hai tu hamaa , struct lagana parta hai. 


# structure vs array


| **structure**                                              | **array**                                                               |
| ---------------------------------------------------------- | ----------------------------------------------------------------------- |
| structure different types ka data store  bhi kar sakta hai | array aik kissam ka data store karti hai                                |
| structure ma majood har variable ka name hota hai.         | array ma variables ka name nahi hota hai balka un ka index no hota hai. |
| ya bhi group of variables hota hai                         | ya bhi group of variables hota hai                                      |

# intialization

![[Pasted image 20240718121101.png]]


![[Pasted image 20240718121020.png]]
>[!tip]- member access
> .(dot)   ko hum bolta hai member access operator


# taking input from user

![[Pasted image 20240718121757.png]]

# structure array

![[Pasted image 20240718121722.png]]

# function returning structure

![[Pasted image 20240718121957.png]]

![[Pasted image 20240718122432.png]]


# buffer

standard input output devices ka wo area jaha in ki  values temporarily ja kar store hoti hai.

![[Pasted image 20240718172726.png]]

![[Pasted image 20240718172805.png]]
![[Pasted image 20240718173222.png]]
![[Pasted image 20240718173258.png]]


# fflush

jab hum character or string input lena sa pahlaa koi input laa, tu usss sa input buffer barh jata hai, jab input buffer barh jata hai tu agar tab hum character ya string input la ga tu issue ho ga, jisss ka liya hum, fflush(stdin) sa input buffer ko free karaa ga.


# structure pointer

jab hum structure variable ki madad sa member variable ko access karaa ga tu hamaa (dot .) lagana paraa ga

laikin jab structure pointer ki madad sa member variable ko access karaa ga tu hamaa (arrow ->) lagana paraa ga.


![[Pasted image 20240718174628.png]]

(asterik p) iss waja sa likha hai takaa ya pahla b1 bann jaye. agar brackets nahi lagaye ga tu pahlaa dot solve ho ga kio ka usss ki priority zayada hoti hai.


