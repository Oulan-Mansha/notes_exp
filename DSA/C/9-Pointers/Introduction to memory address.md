
- **Koi bhi program jab run hota hai tu ussaa RAM ma jagha milti hai.** 
- **Kitni milti hai ya baat important nahi hai.** 
- **iss ma aik aik byte kar ka lakho bytes hota hai.** 
- **humm un bytes ko 0 base counting ka mutabiq count karta hai.** 
- **jab ham aik variable banata hai tu wo lagatar ma 4 bytes leta hai. Or jab uss ka address pahla bytes ka address ho ga.** 

![[IMG_20240713_121937.jpg]]


# Referencing and derefrencing

- variables ka kia address ho ga wo operating system decide karta hai. 

**&-> address of operator apna operand (variable) ka address batata hai. 

- ham printf ma directly address nahi likh sakta kio ka hamaa pata hi nahi hota ka variable ka kia address ho ga.
- *& right to left solve hota hai.

![[Pasted image 20240713143818.png]]

![[Pasted image 20240713144831.png]]


![[Pasted image 20240713153849.png]]

- decleration ka waqt jab hum varaible ka sath asterik lagata hai tu wo sirf aik symbol hai jo compiler ko batata hai ka ya amm variable nahi hai or iss variable ma jo integer rakha jaye ga wo integer nahi ho ga balka wo aik variable ka address ho ga.
- decleration ka waqt jab hum variable ka sath asterik lagata hai tu wo variable pointer variable ban jata hai.
- decleration ka baad jab hum ussi variable ka sath asterik lagata hai tu pointer variable wo variable ban jata hai jissaa wo point kar raha hota hai.

# pointer

![[Pasted image 20240713154030.png]]

# size_of_pointer


![[Pasted image 20240713160009.png]]

- **aik program ko run hona ka liya kitni memory milti hai ya OS ki generation par depend karta hai.

![[Pasted image 20240713160820.png]]




# base address

![[Pasted image 20240713174757.png]]



# data type of variable

**jiss typa ka pointer hai, ussi type ka variable ka address uss ma rakhna chahye, agar aissa nahi karta tu galat ho ga. laikin koi error nahi aye ga.

>[!tip]- reason:
humm janata hai ka pointer base address ko store karta hai, agar humm integer pointer or integer ki baat karaa, tu integer pointer base address ka aglaa walaa teen bytes ko access kara ga, chahee usss ma integer variable ka address store ho ya phir character variable,jab humm uss ma character variable ko rakha ga tu wo base address sa aglaa teen bytes ko access kara ga jo ka illegal memory access ho ga. or jab illegal memory acccess hota hai tab program execute bhi ho sakta hai or crash bhi.  


![[Pasted image 20240713175940.png]]


in above pic, "r" double ka variable ko point kara ga, matlab ya double type ka variable ka base address store karaa ga, or uss base address ka agaa 7 bytes ko access kara ga. same for char, int.


# Extended Concept


![[Pasted image 20240713183128.png]]


#### Double pointer :
	agar hum asterik q likha ga tu ya nahi pata challa ga ka ya ordinary variable ka address store karaa ga, Ya phir kissi dossraa pointer variable ka address store karaa ga. issi liya hum usss ka sath double asterik lagaye ga.

#### level of pointer

pointer variable ka sath humm jitna star lagaye ga wo variable utna level ka ho ga.

jaisaa ka r-> three level pointer , q -> two level pointer , r-> one level pointer , x -> zero level pointer(no pointer)

