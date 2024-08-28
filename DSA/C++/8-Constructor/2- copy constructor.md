
jab hummm object banaa rahaa hota hai, orr ussi waqt hummm ussi object ko usssi ka class ka object sa intilize karwaa deta hai tu copy constructor call hota hai.

```
#include <iostream>

using namespace std;

class complex{

int a,b;

public :

void set_data(int x,int y)

{

a = x;

b = y;

}

void show_data()

{

cout<<a;

b<0?cout<<"":cout<<"+";

cout<<b<<"i";

}

complex add(complex);

complex(){a=0,b=0;}

complex(int x){a=x,b=0;}

complex(int x,int y){a=x,b=y;}

  

};

  

complex complex::add(complex C)

{

complex temp;

temp.a = a + C.a;

temp.b = b + C.b;

return temp;

}

  
  

int main()

{

complex c1(2,4),c2(2),c3;

complex c4 = c1; // here copy constructor will be call

c4=c1; // here assignment operator will do operation

  

}
```

![[Pasted image 20240801124819.png]]


![[Pasted image 20240801114158.png]]

we write & or asterik in formal arguments of copy constructor to avoid recursion.

```
#include <iostream>

using namespace std;

class complex{

int a,b;

public :

void set_data(int x,int y)

{

a = x;

b = y;

}

void show_data()

{

cout<<a;

b<0?cout<<"":cout<<"+";

cout<<b<<"i";

}

complex add(complex);
 

complex(){a=0,b=0;}

complex(int x){a=x,b=0;}

complex(int x,int y){a=x,b=y;}

complex(complex *C)// (complex &c)

{

a = C->a;

b = C->b;

}

  

};

  

complex complex::add(complex C)

{

complex temp;

temp.a = a + C.a;

temp.b = b + C.b;

return temp;

}

  


  

int main()

{

complex c1(2,4),c2(2),c3;

complex c4 = &c1; // here copy constructor will be call

c4.show_data();

  
  

}
```


- hummm na jab deep copy karni ho gi, tabb hameshaa copy constructor hamaa banana paraa ga.



## shallow copy vs deep copy



![[Pasted image 20240801135417.png]]


#### shallow copy 

- isss ma ya ho ga aik object ka variables ka data doosra object ka variables ma chalaa jaye ga. matlab (above pic ma ) **p** ma jo address hai wo dosraa object ka **p** ma store ho jaye, or doosra object ka **p** usssi address(memory block) ko point karaa ga jissaa pahlaa object ka **p** kar raha hai. isss ka nuqsaan ya ho ga agaar pahlaa object ka **p** ka zariyaa memory block ki value ko change karaa ga, tu wo doosra block ka **p** ka lia bhi change ho jaye gi. 
- laikin agaar humm chahtee hai ka doosraa object ka **p** kissi doosra memory block ko point karaa, magaar usss ma value, pahla block walaa **p** ki a jaye tu hummm deep copy karaa ga.
- complier jo copy constructor banataa hai usss sa ya hota hai.

#### deep copy


![[Pasted image 20240801135725.png]]
