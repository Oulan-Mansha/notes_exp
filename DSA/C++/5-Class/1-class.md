agaar hummm struct ki jghaa class likh da ga tu wo class bann jayee gi.

c++ ma jo **struct** ka zariaa kar sktaa hai wohi **class** ka zariyaa kar sktaa hai.


**phir dono c++ ma kio majood hai jab dono sa same kaam ho skta hai :**

c++ C ka superset hai, lahzaa jo C ma struct ka sath humm kar sakta hai wohi c++ ma bhi struct ka saaath kar sakta hai (takaa backward compatibilty maintain rahaa), laikin jo additional ayiii wo optional rakhi gai thi.

c++ ka developers naa socha ho sktaa hai, oop ka aissaa concepts aa jayee jinn sa backward compatibility maintain na rahaa tu unho na isss mushkil sa bachna ka lia aik naya concept hi introduce karwa dia (class) , ya C ma nahi thaa, lahazaa backward compatibility ki musibaat hi khataam hoi. unho na soochaa agaaar oop ka koi new concept ayee ga, agaar usss ki wajaa backward compatibility maintain na rahaa gi tu hummm usssaa struct ma introduce nahi karwaye gaa balka class ma introduce karwa da ga.

**diff b/w class and struct**

- struct ka tamaam members by default public hota hai, matlab hummm unhaa bahir sa access kar sakta hai, jo ka C ma hota hai, (iss public concept nahi hota), lahazzaa backward compatibility ko maintain karnaa ka liaa ya karnaa paraa.
- class ka tamaam members by default private hota hai. 


```
#include <iostream>

#include <string.h>

using namespace std;

class book{

// they are by default private

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

structure variable ko hi object kahta hai.

>[!note]- important note
>jitni bhi object oriented languages hai, unn ma class ka concept hai, structure nahi hai. lahazaa hummm c++ ma bhi class hi use karaa ga. laikin jo kaam humm class sa kar skta hai wo structure sa bhi kar sakta hai.



![[Pasted image 20240729154121.png]]


-  **2nd last point :**  jaissaa aik makaan banana hotaa hai, humm uss ka naqshaa banaa letaa hai, uss ka baad usss naqshaa ko daikh kar humm jitnaa chahaaa makaan banaa saktaa hai, aissaa hi humm aik class banataa hai, phir usss class sa jitnaa chahaaa objects banaa leta hai.
- **3rd point :**  aik object kon kon sa variable ko access kar skta hai, kon kon sa functions ko call kar skta hai, yaa humaa class ko daikh kar pata chala ga.
 
 

![[Pasted image 20240729154701.png]]
