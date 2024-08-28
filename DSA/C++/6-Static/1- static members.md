![[Pasted image 20240730092238.png]]

![[Pasted image 20240730103404.png]]

- function call hona sa pahlaa static local variable ko memory mil jati hai, function end hona ka baad bhi static local variable ki memory release nahi hoti.

- scope -> variable kaha kaha sa accessible hai.

### static member variable:

- static member variable -> class variable (kio ka ya poori class ko belong karta hai).
- instance variables ko declare karna sufficient hai, jab koi object banaye ga tu inha bhi memory mil jaye gi.
- static member variables ko declare karna sufficient nahi hai, jab inhaa define karaa ga or object banaye ga, tab ja ka inha memory mila ga

- inha humm define class ki body ka bahir karta hai.
- yaa object ka variable nahi hai, isss ka matlab ya object ma nahi banta hai, balka ya class ka variable hai. aik class ka saraa variables ka lia memory alaag sa milti hai.
- isssaa aik hi baar jaghaa milaa gi pori class ka andaar, chahee usss class ka aik object ho, 10 object ho ya koi object na ho, issaa aik dafaa jagha milaa gi.

```
#include <iostream>

using namespace std;

class Item{

public:

int a,b; // instance variables

static int k; // static member variables / class variables

  

};

  

int Item::k; // defining static member variable || or jab hum ya line likhaa ga tab k ko value mila gi.

int main()

{

Item it1,it2;

it1.a=5;

cout<<it2.a;

cout<<endl;

it1.k=2;

cout<<it2.k;

cout<<endl;

return 0;

  

}
```

![[Pasted image 20240730115146.png]]

```
#include <iostream>

using namespace std;

class Item{

public:

int a,b; 

static int k;

  

};

int Item::k;  // k class ka variable hai, isss wajaa sa hummm issaa class name               sa access kar skta hai.

int main()

{

//Item it1,it2;

//it1.a=5;

//cout<<it2.a;

//cout<<endl;

Item::k=2;

cout<<Item::k;

cout<<endl;

return 0;

  

}
```


![[Pasted image 20240730120023.png]]



#### public static member variable :

![[Pasted image 20240730150854.png]]

- 2sraa tareeqa bahtar hai kio ka hummm static member variable ko tab bhi access kar skta hai jab koi object na bana ho.
- agar hum objectdot lagaa kar static member variable ko access kara ga tu aissaa lagaa ga ka static member variable usss object ka member, jo readability ka lahaz sa mushkil, ya confusion paidaa kar skta hai.

#### private static member variable :

above mention

```
#include <iostream>

using namespace std;

class Item{

private:

  

int a,b; // instance variables

static int k; // static member variables / class variables

public:

  

void set_a(int n) {a=n;} // instance method

void set_b(int m){b=m;} // instance method

int get_a() {return a;} // instance method

int get_b() {return b;} // instance method

void set_k(int l) {k=l;} // instance method

int get_k() {return k;} // instance method

};

  

int Item::k; // defining static member variable || or jab hum ya line likhaa ga tab k ko value mila gi.

int main()

{

Item it1,it2;

it1.set_a(5);

cout<<it2.get_b();

cout<<endl;

it1.set_k(10);

cout<<"k = "<<it2.get_k();

cout<<endl;

return 0;

}
```




- wo function jo object specific kaam na karaa, matlab object members ko use na karaa, usssa static method banaa da ga. yaa phir taab banaye ga, jab function instance variables ko access na karaa or sirf static member variables ko access karaa.
- instance method tab banaye ga jab method instance variables ko access kar.
- instance method static member variable ko access kar skta hai.
- static method instance variable ko directly, access nahi kar skta kio ka jab static method ko object banaye baghaair access kar skta hai, or jab object banaa hi nahi or agar static method instance variable ko access karaa ga tu isss sa ya pataa nahi chalaa ga ya kon sa object ka instance variable ko access kar raha hai, iss mushkil sa bachna ka lia yaa kia gia hai.


```
#include <iostream>

using namespace std;

class Item{

private:

  

int a,b; // instance variables

static int k; // static member variables / class variables

public:

  

void set_a(int n) {a=n;} // instance method

void set_b(int m){b=m;} // instance method

int get_a() {return a;} // instance method

int get_b() {return b;} // instance method

static void set_k(int l) {k=l;} // static method

static int get_k() {return k;} // static method

};

  

int Item::k; // defining static member variable || or jab hum ya line likhaa ga tab k ko value mila gi.

int main()

{

//Item it1,it2;

//it1.set_a(5);

//cout<<it2.get_b();

//cout<<endl;

Item::set_k(10);

cout<<"k = "<<Item::get_k();

cout<<endl;

return 0;

  

}
```

![[Pasted image 20240730151154.png]]

##### example :

![[Pasted image 20240730151614.png]]
