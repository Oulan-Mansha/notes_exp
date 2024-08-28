
![[Pasted image 20240705161912.png]]

![[Pasted image 20240705162055.png]]

![[Pasted image 20240705162649.png]]

- In programming we can't write variables in the form of sub_script directly, there for we use array for this purpose.
- array ka saraa variables lagataar ma memory consume karaa ga.(means in memory they are store in contiguous form) / (in memory they are adjacent memory blocks).
- array is a group of same type of variables (it's not possible that one element of its int, one is float and one is char).
- array collectively has name but elements doesn't have name.

![[Pasted image 20240705171143.png]]


![[Drawing 2024-06-27 19.44.46.excalidraw|1000]]

- to access array variable we write array variable index in subscript operator.

a[3] is not a variable. it's an expression, which has one operator [] and two operands a,3. 
its (a[3]) result becomes the representation of 4th memory block(above pic) in (a[3]) which 25 will be assign . a[3] is the expression which represent 4th memory block.

- we can use loop to access array elements because array elements doesn't have any name, array element represent by expression, whose one operand is index and we can change that operand with the help of loop.



## array deceleration

![[Pasted image 20240705175929.png]]

![[Pasted image 20240705180545.png]]

5- compiler give that error (it is a deceleration statement which is handle by compiler, therefore it give an error at compile time).

![[Pasted image 20240705180711.png]]
![[Pasted image 20240705181614.png]]
- compiler will count the values (above compiler will suppose 5 at square brackets).

>[!tip]- bug
>logical errors

![[Pasted image 20240705194948.png]]

>[!tip]- bound checking
> - determining / checking whether array accessing more memory elements than it reserve.
>it is done by compiler. (Array bound checking refers to **determining whether all array references in a program are within their declared ranges**.)
> - it is done by compiler at compile time. but it will check only for declaration statement and will give error.
> - compiler will not give error for action statement and at the time of execution the program will terminate when it will access memory more than it reserve at the time of declaration.



