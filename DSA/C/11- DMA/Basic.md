
data ko process karna ka lia humm program banata hai, uss processing ka duraan hamaa data ko kahi preserve kar ka rakhna parta hai, isssi waja sa variable banataa hai.

variables do tariqo sa banta hai :

# 1- SMA (Static Memory Allocation):

jitna bhi variables haamm declaration statements sa banata hai wo sab ka sab SMA ka under ataa hai.
wo memory allocation jo humm declaration statements ka madad sa karwataa hai.
jiss time program compile hota hai uss time declaration statements process ho jata hai or unha program sa hataa dia jata hai. ya sirf compiler ka lia banata hai, usss ka baad jab exe file banti hai tab yaa usss ma nahi hoti.
Declaration statements ko daikh kar compiler ya taaah karta hai :
	1- Program ma kitna variables hai.
	2- unnn variables ka type kia hai.
	3- unn ma kiss tarha ki value store ho sakti hai.
	4- unnn ka size kia ho ga.
	5- unnn variables ka lifetime kia ho ga.
	6- unn variables ka scope kia ho ga.
	7- variables ko kitni memory mila gi.
	
yaa saab cheeza compiler compile time par karta hai. or compiler inn sab cheezo ko exe wali file ma likha deta hai.
SMA walaa variables ma humm runtime ma kuch change nahi kar sakta hai.

program jab run hota hai tab hi program ko memory allocate hai or taab hi inn variables ko bhi memory milti hai.

SMA wala variables ka kio na kio name hota.

# 2- DMA (Dynamic Memory Allocation)

wo variables jo humm action statements sa banata hai wo DMA ka under ataa hai.
wo memory allocation jo humm action statements ka madad sa karwataa hai.
					ya
jo variables calloc() or malloc() function sa banta hai, wo DMA ki category ka under ata hai.
jabb calloc() ya malloc() ko call kartaa hai tab variable banta hai, or function call action statement hi hotii hai.
DMA walaa variables action statement sa banta hai, iss waja sa compiler inha excecute nahi karta or na koi bhi decision leta hai. wo sab kaam run-time par hota hai.
DMA walaa variables ka koi name nahi hota.
DMA walaa variable ko agar free ma karayaa jaye tu uss ka lifetime till the end of program hota hai.

![[Pasted image 20240718194737.png]]



# malloc


malloc ma humm jo size da ga, wo usss size ka variable banaa da ga.
koi tariqa nahi malloc ko batana ka kiss type ka variable banana hai.
yaa kissi bhi type ka variable nahi banata, ya basss usss size ka variable banaa deta hai jisss ka size isssa dia jata hai.
malloc void type ka address return karta hai.
e.g :
abb humaraa pass aik unknow type ka variable ka size a gaya, humaa pata hai ka humm na ussaa integer ki tarha treat karna hai, tu hum SMA ka through aik intger pointer bana da ga. jab humm usssaa koi address da ga tu wo yaa maan ka chalaaa ga ka mera pass integer type ka variable ka address hai.laikin hamarraaa pass jo variable hai usss ka type tu void hai, laikin pointer integer type ka hai, jiss ki wajaa sa type-mismatch ka error aye ga.

![[Pasted image 20240718201051.png]]

# type_casting

![[Pasted image 20240718201759.png]]

humm na sirf ordinary integer value nahi banana balka int type ka variable ka address banana hai tu iss waja sa star lagana paraa ga.

# calloc

calloc array banata hai. iss sa lagatar ma multiple variables banta hai.
iss ma wo array ka pahla block ka element ka address return karaa ga.

![[Pasted image 20240718202247.png]]

pointer agar int type ya float type ka hai tu wo 4 4 byte kar ka hi memory ko access karaa ga tu lahaza jo kaaam calloc ma kar raha hai wohi malloc ma karaa ga.


# malloc vs calloc

![[Pasted image 20240718202556.png]]
