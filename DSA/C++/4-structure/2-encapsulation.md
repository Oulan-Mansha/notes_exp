
- Agar hamaraa pass mukhtalif cheeza hai or humm unn ko cover kar dia, wrap up kar dia, unn ka gird aik boundary bana dii. Tu hummm kaha ga humm na unnn cheezo ko **encapsulate** kar dia hai.
- Kuch cheezo ka group bana dena. 

- Jaisaa aik capsule hota hai, wo apna andar powder ko ikhata kar ka rakhti hai. Uss powder ki koi boundary hai. Issi sa hai encapsulation.


![[Pasted image 20240728191843.png]]


**Technical Definition :**
	aisaa kaaam jisss ma kissi bhi entity ki properties or actions/methods ko combine kar ka group banana encapsulation kahlata hai. 

**Entity :** 
         Har wo cheez jisss ki independent existence ho and jiss ki koi properties hai.


1- hum structure ma jo functions banaye ga jo structure ma majood variables ko use karaa ga.
2- agar entity sa related saraa variables or saraa functions ko combine karaa ga tab hi humm kaha ga ka humm na encapsulation ki hai.agar aik bhi function usss combination na howaa bulka structure sa bahir banaya tu wo encapsulation nahi ho ga.

#### encapsulation rules
 
 - jab humm koi function structure ka andar define karaa ga tu usss ka declaration structure sa bahir nahi karaa ga or ya member function kahlaye ga kio ka ya function structure ka andaar hai.
 - usss function ko dot lagaa kar access kar sakta hai.
 - ya function jiss structure ma bana hai, uss structure ka member variables ko access kar sakta hai.
 
 ```
#include <iostream>

#include <string.h>

using namespace std;

struct book{

int bookid;

char name[30];

float price;

void output(book b)

{

cout<<b.bookid<<" "<<b.name<<" "<<b.price;

}

};

book input()

{

book b;

cout<<"Enter book id : ";

cin>>b.bookid;

cout<<"Enter book name :";

cin.ignore();

cin.getline(b.name,30);

cout<<"Enter book price : ";

cin>>b.price;

return b;

}

int main()

{

book b;

b = input();

b.output(b);

cout<<endl;

return 0;

}
```

agaaar humm likhta hai, ramesh.running() iss ka matlab jo paaoo hai wo ramesh ka dard ho ga, ya phir agar humm likhaa ga shahid.studing() tu faidaa oulan hi ka ho ga.

isssi tarha jaab humm likhaa ga b.output() tu output b hi ki show ho gi.

```
#include <iostream>

#include <string.h>

using namespace std;

struct book{

int bookid;

char name[30];

float price;

void output()

{

cout<<bookid<<" "<<name<<" "<<price;

}

};

book input()

{

book b;

cout<<"Enter book id : ";

cin>>b.bookid;

cout<<"Enter book name :";

cin.ignore();

cin.getline(b.name,30);

cout<<"Enter book price : ";

cin>>b.price;

return b;

}

int main()

{

book b;

b = input();

b.output();

cout<<endl;

return 0;

}
```


humm na C language sa parhtaa a raha hai ka member variable ki khud ki identity nahi hoti, lahazaa humm unnn ka aissa hi nahi likh sakta.

C++ ma member variables ko directly likh skta hai, laikin sirf unnn ka structure ka member function ka andar ya structure ki body ka andar.

above example ma : jo structure variable(b3) member function(output) ko access karaa , tu member function(output) structure variable(b3) ka member  variables ko access karaa ga.

```
#include <iostream>

#include <string.h>

using namespace std;

struct book{

int bookid;

char name[30];

float price;

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
