# Checkpoint Answers Chapter 2 #
**2.1**  
The problem with the original code, presented in the book, is that the string to be printed is split with an end-line. This is not allowed.  

The solution is to use string concatenation. Most development environments will actually insert this automatically for us these days.  

A fixed version of the code looks like this:  
```Java  
public class Test {

	public static void main(String[] args) {
		double i = 50.0;
		double k = i + 50.0;
		double j = k + 1;
		
		System.out.println("j is " + j + " and "
				+ "k is " + k);

	}

}  
``` 

**2.2**  
The Scanner class can be used for getting input from the user. An import of this class is required and the class can then be used in this way:  
```Java
Scanner input = new Scanner(System.in);
double number = input.nextDouble();
```  
The above code expects the user to enter a number. Should the user write something else like 5a so will this cause a so called Exception. This Exception must be handled in the code because the program will otherwise terminate in an uncontrolled manner.  

**2.3**  
There are no performance differences between the following two import statements.
```Java  
import java.util.Scanner;
import java.util.*;
```  

