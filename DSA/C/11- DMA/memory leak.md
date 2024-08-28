
![[Pasted image 20240718203558.png]]

jab programmer heap ma memory reserve karwataa hai or ussaa delete karna bhool jaye tu ussa memory leak.
isss ka nuqsaan ya hota hai kaa humm usss memory ko access nahi kar pata or wo memory wastage ka farizaa nibhati hai.
agaar aissi galti zayadaa bhaar ho jaye tu memory ki kami bhi ho sakti hai. 


# solution (free)

agar ap ko memory leak sa bachna hai tu free function use karna paraa ga.

![[Pasted image 20240718205118.png]]

![[Pasted image 20240718204930.png]]

![[Pasted image 20240718205519.png]]
![[Pasted image 20240718205657.png]]

# realloc 

isss sa hum malloc or calloc sa banai hoa, variable / array, ko resize kar sakta hai.
jo ya resize kar ka hammaaa address da ga hummm ussaa pahlaa walaa pointer ma bhi rakh sakta hai or new pointer bhi bana sakta hai.
or realloc ko jo address diya jaye ga woo uss memory ko bhi free kar da ga or previous data ko bhi resize howa variable / array ma rakhwaa da ga.


![[Pasted image 20240718210632.png]]
