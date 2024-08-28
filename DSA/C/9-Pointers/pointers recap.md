
![[Pasted image 20240715150436.png]]


# pointer's arithmetic

 agar ap do adresses ko add, multiple, ya divide ki koshish karaa ga tu error aye ga.

![[Pasted image 20240715153131.png]]


![[Drawing 2024-07-15 15.19.05.excalidraw|5000]]

>[! tip]- subtraction
jab hum do addresses ko pointers ki help sa subtact karta hai, tu address ko subtract karna ka baad jo result ata hai ussa(e.g. 1000 answer aya 1000 ma kitna 4 4 bytes ka address ho ga wo hum 4 sa divide kar ka pata kar la ga), size of type of pointer sa divide karta hai, uss ka baad jo result hota hai wohi answer hota hai.  (pointers ka type same hona chahye.
pointers ko subtract karna ka baad jo result ata hai wo address nahi hota.
or uper negative 250 sirf direction bata raha hai. ka choti value ma sa bari value ko subtract kia hai.



# swap

![[Pasted image 20240715183453.png]]


# scanf

hummm kissi bhi doosra function ko apna function ka variable ka address iss waja sa deta hai taqaa wo hamaraa function ka variable ko pointer ki madad sa access kar saka , uss  ma kuch changes kar saka.


hum scanf() function ma & iss waja sa likhta hai takaa scanf() function ko hamaraa variable ka access mila or wo hamaraa variable ma data ko store kar sakaa.





# array of pointers


![[Pasted image 20240716071011.png]]

2d array tab banata hai jab , buhat saraa data ko aik hi jagha par rakhna ho or uss ka size or type same ho **or**  har 1d-array ka data same size ka hota hai(ya unn ki length same ho) or data real world ma bhi 2d ho.


![[Pasted image 20240716082002.png]]

# pointer to array


ya 2d array ko access karna ka liya istamal kia jata hai.

![[Pasted image 20240716114701.png]]

![[Pasted image 20240716115304.png]]


# wild pointer



![[Pasted image 20240716120501.png]]


jab hum pointer banata hai or ussa initialize nahi karta tu ussss ma garbage value hoti, jo ka program ka kissi byte ka address ho gi, pointer ko kissi variable ka address dia baghaair jab hum ussa koi value assign karaa ga, tu pointer apna andar majood memory address par value rakhwaye ga, jo ka illegal memory access ho ga kio ka hummm na ussa memory address ko reserve hi nahi kia thaa, or jab hum illegal memory access karta hai tu uss sa program crash ho jata hai.


# NULL pointer

NULL ka meaning stdio.h ma declare hai.
NULL -> 0
jab humm kissi pointer ko NULL(0) assign karta hai tu wo program ko jo memory mili hai iss ka  pahla block ko point karta hai, laikin hummm ya manta hai ka wo kissi ko point nahi kar raha hai.

hum pointer ma null iss wajaa sa assign karta hai taka wo wild pointer na raha.


![[Pasted image 20240716122239.png]]


# Dangling pointer


![[Pasted image 20240716122149.png]]

![[Pasted image 20240716122904.png]]
![[Pasted image 20240716123337.png]]


# void pointer

void type ka hum normal variable nahi bana sakta laikin pointer variable bana sakta hai.

![[Pasted image 20240716123658.png]]

![[Pasted image 20240716123942.png]]

agar typecast kia baghair derefrence karaa ga tu error aye ga kio ka pointer ko nahi pataa ka wo kiss type ka block ka address hai. 


agar hum *(int)p likh da tu p ma rakha address normal integer mana jaye ga, laikin humm chahte ka p rakha address, address mana jaye tu hama *(int *)p likhna para ga.