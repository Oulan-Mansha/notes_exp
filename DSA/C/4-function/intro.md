
![[Pasted image 20240629123737.png]]

	it reduces no of lines because we don't need to write same lines again and again, we can just call the functions.
## function body
	it is that place where you write code

![[Pasted image 20240629124944.png]]

## function call

	we can say that it is representative of function defination because when we call function then all statements which we write during function defination will be execute and that function will be load into memory.
	


![[Pasted image 20240629130604.png]]




![[Pasted image 20240629160003.png]]


>[!tip]+ imp
>main is user define function because we define it.(we write its name and code in its block{curly opening and closing brackets})


## flow of program


![[Pasted image 20240629171130.png]]


![[Pasted image 20240629170644.png]]

- when we call the function, the function loads into the RAM, when all the statements in it execute then function remove/delete from memory and after that control transfer to that location from where the function has been called by considering that line has been execute so that's why next line executes. 
- free area + consumed area = same (at any point of time)  ---> because total memory is fix.  (equal memory(RAM) gives to every C program.)
- function gets its memory when we call it (either it is globally declare or locally declare).-> it is totally opposite.
- when we declare functions locally then we can only access it in that function where it is declare. it can't be access by other function.
- if we want that other functions access them then we have to declare it globally


![[Pasted image 20240629173852.png]]

![[Pasted image 20240629174009.png]]


## ways to define a function

- takes nothing return nothing
- takes something return nothing
- takes nothing return something
- takes something return something


![[Pasted image 20240629190713.png]]



- actual arguments data copies into formal arguments


![[Pasted image 20240629194205.png]]


![[Pasted image 20240629194522.png]]

![[Pasted image 20240629194936.png]]

![[Pasted image 20240629194745.png]]

library file will contain compiled code, so you can't see source code.
function prototype = function deceleration
10- yes, we can call main function,may be our program becomes never-ending but using tricky condition we can terminate it.but we don't call main function because by this our program becomes messy.