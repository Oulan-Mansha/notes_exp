![[Pasted image 20240627190436.png]]

>[!tip]+ important
> - in above image, constants must be different(it is a rule)
> - in while() and if() parenthesis, we writes condition which evaluates to true or false.But    here(switch),we write expression(piece of code i.e. combination of variables,literals,operators and function call) which return single value after evaluation.
> - the expression which we write in switch parenthesis, always returns a integer value,which is possibly always written in-front of case.
> - we move to the default case, when none of the case constant match with switch expression's result.



>[!note]+ most important
>The switch statement is more efficient than the if-else structure when comparing a single variable or expression to multiple constant values because **it directly jumps to the matching case instead of evaluating each condition in a sequential manner as in the if-else structure**.
> - in other terms we can say that, it says move to that case whose constant = expression result.
> - its work is just to move processor control to that case whose constant = expression result.




![[Pasted Image 20240627194547_057.png]]



![[Drawing 2024-06-24 08.38.23.excalidraw|50000]]







![[Pasted image 20240627200719.png]]


#### 1st point of above pic

![[Pasted image 20240627200017.png]]

### last point of above pic

![[Pasted image 20240627203713.png]]


# nesting

we can do nesting,by writing switch in case.


# ranges 

we can define ranges in case, by writing three dots(...) between range 1 and range 10.
there must be one space between range and dotes.

```
 switch(x)
 {
	 case 1 ... 10:
		 printf("gg");
	 case 2 ... 20:
		 printf("ahm");
 }
```

# exit

this function is used to forcefully terminate/kill the program.in its parenthesis we write 0, which indicates/ send message,after terminating program, to OS that our program has been run successfully and know we want to terminate our program. while if write 1, it sends message to our operating system that our program has not been run successfully and now it has been terminated. (2:24-2:27) 


![[Pasted image 20240627210449.png]]


###### we can write any number of labels(پَرْچی لگانا      عنوان)(label means giving name to line) in the program but they must have different names

###### it is strongly recommend that we shouldn't use goto because it doesn't have confined body unlike while and if. moreover, it makes complexity in the code. it doesn't use in today's language.
###### it just move the control to the label location.



![[Pasted image 20240627211042.png|left]]

![[Pasted image 20240627211236.png]]


![[Pasted image 20240627211751.png]]
