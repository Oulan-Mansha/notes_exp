functions memory efficient hota hai, wo aissa ka jab inha call karta hai ya tabb hi RAM ma ataa hai, or execute hona ka baad ussi time RAM sa remove ho jata hai.

**disadvantage :**

jab koi function kissi doosra function ko call karta hai, tu pahla function apna status ko preserve karta hai, doosraa function RAM ma load hota hai, uss ka code chalta hai, jab wo apni lines execute kar leta hai, uss ki memory ko free kia jata hai, or dobaraa calling function ko resume kia jata hai, ya saab extra kaam karna parta, isss sa execution time barh jata hai. program zayda time leta hai.


![[Pasted image 20240720114451.png]]
![[Pasted image 20240720114805.png]]
![[Pasted image 20240720114840.png]]
![[Pasted image 20240720120054.png]]

- compiler ka hisaab sa aghar **inline function** kam memory laa ga tu wo usssaa, compile hona ka baad jo file banti hai usss ma whaa likh daa ga jahaa sa ussaa (function) call kia gia hai.laikin source file ma kuch change nahi ho ga. Isss ka faida ya ho ga ka function ko runtime par call nahi karna paraa ga.
- program ko kitni memory mila gi, ya compiler ko tu pata nahi. isss wajaa sa kuch conditions ki bunyaad par function ki memory ko judge karaa ga, wo conditions uppar mention hai.

![[Pasted image 20240720131654.png]]

