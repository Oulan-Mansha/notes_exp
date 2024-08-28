
- means data ko chupanaa , ya phir access nahi karna dena.
- ya feature c ma nahi hai, sirf c++ ma hai.

**Example :**

![[Pasted image 20240729100411.png]]

farz karaa humm na do variables banayee or unn ma jo data hai, wo 2 sa 3 functions use karna chahtaa hai, tum humm C ma unha global bana da ga.Laikin humm chahtee hai, unnn 2 sa 3 functions ka ilaawa koi or function unn variables ka data ko access na karaa. Tu isss ka lia C ma koi feature nahi hai, C++ ma isss ka lia feature hai, jissaa data hiding kahta hai.

**aisssaaa hum kio chahtaaa hai (Reason):**

agaar humm aik project khud banaa rahaa hai tu unn variables ko use karnaaa ya nahi karnaa wo humm decide kar sakta hai.Laikin agar hum baraa project banaaa rahaa hai, jisss ma buhaat saraaa programmers ho ,jiss ma teeen function koi or banaa rahaa hai or neechaa walaa 2 function koi orrr banaa raha hai.

 humm chahtaa hai ka wo teeen functions unnn variables ko access karaa lahazaa humm na un variables ko global banaa dia, joo ooper wallaa 3 functions banaa rahaa hai, unn ka problem domain alaag hai, or jo neechaa 2 functions banaa rahaa hai, un ka problem domain alaag hai.
 jo neechaa walaa functions banana walaa programers thaa unhaa lagaa agar humm unn variables ko access karaa ga tu hamaraa faidaa ho ga, laikin wo nahi jantaa thaa unn variables ma kia rakhwaaa skta hai, lahazaa unho na apnaa hissaaab sa data rakhwaa dia. jisss sa data corrupt ho skta hai.
 
agaar humm baraa program bana raha hai tu yaa possible nahi hai, har programmer ko ya pataa ho ka har variable ki kia policy hai.

>[!tip]- data corrupt
>- jaab humm variable ma aissa data rakhwaye ga jo data ki policy ka khilaaf ho ga, tu usssaa kahaa ga data corrupt ho gaya hai.
>- let's say humm na policy banaye thi ka variable ma sirf even numbers store ho ga, laikin agaar humm usss ma odd number rakhwaaa da ga tu humm kahaa ga kaa variable ka data corrupt ho gaya hai.



![[Pasted image 20240729104857.png]]


>[!imp]- data hiding
>- not allowing you to access some of the members of the structure by making them private.
>- kuch members ko har jgha sa access nahi kia ja sakta.
>- data ka access na dena.
>- structure members ko hide karna. unnn ka scope batanaa ka unnn ko kaha sa access kia ja skta hai.
>- ya humm access modifiers sa karta hai.

>[!tip]- access specifiers
>- private members sirf structure ma hi access kia ja skta hai.
>- public members puraa program ma access kia ja skta hai.


```
#include <iostream>

#include <string.h>

using namespace std;

struct book{

private:

int bookid;

char name[30];

float price;

public:

void output()

{

cout<<bookid<<" "<<name<<" "<<price;

}

void input()

{

cout<<"Enter book id : ";

cin>>bookid;

cout<<"Enter book name :";

cin.ignore();

cin.getline(name,30);

cout<<"Enter book price : ";

cin>>price;

}

};

  

int main()

{

book b;

b.input();

b.output();

cout<<endl;

return 0;

}
```


>[!imp]- abstraction
>hiding implementation details of any method in the class / structure.

>[!tip]- why we need it
>farz karaa hummm aik baraa program banaa rahaa hai, jisss ma buhat saraa programmers hai,tum koistructure banaa rahaa hai, or ma sirf main() function banaa raha ho,tumm na wo structure banayaa hai uss ki coding tumha pataa, tumhaa usss ka baraa ma zayadaa pataa ho ga, ma na sirf use karna hai,waissaa hi jaissaa, hum "cin cout ko use karta hai, insertion operator" use karta hai, hammaa uss ki coding pataa nahi chalti. ya coding details hummm sa chupai gai hai kio ka wo hamaraa lia unnecessary hai. *just like car, humm basss ya ptaa hota hai, ka accelator ko dabayee ga tu garii chalaa gi, kaissaa ho ga ya zrori nahi hai. soon so forth.basss humm ya janta hai, kia dabayee ga tu kia ho ga, kaisssa ho ga ya janana hamari zarorat nahi hai.*
>humm sirf wo cheezaa nazaar ati hai jinn sa humm na interact karna hai, hamaa gear box dikhta nahi hai, humm sirf gear use karta hai. hummm sirf interface sa interact karta hai.

ooper walaa code ma hummaa pata hai ka agaar humm b.output likhaa gaa tu b ma jo data hai uss ki output show ho gi, laikin kaissaa ho gi ya hammaa show nahi ho raha hai.

chuphana maksaad nahi hai, bass wo unnecessary hai, ap bass ussaa use karo.

![[Pasted image 20240729114450.png]]


