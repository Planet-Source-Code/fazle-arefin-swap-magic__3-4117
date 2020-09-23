<div align="center">

## Swap Magic


</div>

### Description

Do you think it is possible to swap values between two variables without using a third temporary variable? What? No? Yes? Well, the answer is...YES. Take a look at the code and don't forget to vote!
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[FAzle AreFin](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/fazle-arefin.md)
**Level**          |Beginner
**User Rating**    |4.1 (29 globes from 7 users)
**Compatibility**  |C, C\+\+ \(general\), Microsoft Visual C\+\+, Borland C\+\+, UNIX C\+\+
**Category**       |[Math](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/math__3-12.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/fazle-arefin-swap-magic__3-4117/archive/master.zip)





### Source Code

```
/*
	Swapper
	Swaps values between two variables without using a third temporary variable
	Programmer: Fazle Arefin
*/
/*
	use #include <iostream.h> and cout instead of #include <stdio.h> and printf
	if you are using C++, this gives type safety, I didn't use them to keep this
	program C compatible
*/
#include <stdio.h>
int main() {
	int a = 10;
	int b = 20;
	printf("Before swapping a = %d and b = %d \n", a, b);
	a = a + b;
	b = a - b;
	a= a - b;
	/*
		instead of + and - you can use * and / respectively
		a = a * b;
		b = a / b;
		a= a / b;
		instead of + and - or * and / you can use the XOR operator ^
		but this restricts you to only swapping integers
		a = a ^ b;
		b = a ^ b;
		a= a ^ b;
	*/
	printf("After swapping a = %d and b = %d \n", a, b);
	return 0;
}
```

