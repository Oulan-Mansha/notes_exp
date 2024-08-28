
![[IMG_20240709_130610.jpg]]

![[IMG_20240709_130301.jpg]]

![[IMG_20240709_132103.jpg]]

- gets() function have one of the disadvantage that if input string length is more than reserve memory reserve for it, gets() function will put data in reserve memory and as well as free memory and because of it program can be crash or can be execute. 
- basically, it doesn't check whether input string length is less than or equal to reserve memory.  
>[!tip]- gets
>(ya iss baat ka hisaab nahi rakhta ka kitna characters rakha ja sakta hai array ka andar). 

>[!tip]- null character 
>null character string ka ending point hai, agar null character nahi ho ga tu hamaa kaisaa pata chala ka string kaha khatam hoi hai, ya phir usss ki length kia hai. 

 >[!tip]- fgets
 >- ya saab sa safe hai, ya iss baat ka hisaab rakhta hai ka kitna characters array ma rakha ja sakta hai. "\n" is ka liya delimeter nahi hai iss waja sa ya isssa bhi string ma add karta hai. 
 >- it includes the "\n" in the output to remove "\n" we will add "\0".
 
 
![[IMG_20240709_173303 1.jpg]]

 