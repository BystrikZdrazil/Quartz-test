# How to use conditions in C-SHARP
All if statements are either true or false. The condition used for this go in the parenthesis **()**. If the condition is true, the code is executed, else the code is skipped.
## Checking for a single condition
- Testing for equality has to be with **double equals**
- Testing for larger or bigger with the possibility of equality, the **equals sign must be at the end**
- Testing for something that is not equal, we use **!=**
```C#
// checking for equality
if (1 == 1) {
	Console.WriteLine("Inside if");
}

// checking for greater or lesser value
if (2 > 1) {
	Console.WriteLine("Inside if");
}

// checking for greater or lesser value with the possibility of equality
if (age >= 10) {
	Console.WriteLine("Inside if");
}

// checking for greater or lesser value with the possibility of equality
if (age <= 50) {
	Console.WriteLine("Inside if");
}

// checking if it is not equal to something
if (unequals != 8) {
	Console.WriteLine("Inside if");
}
```
We can use **else** statements after an if statement to nest a code we want to execute always when the if statement is false.
```C#
int age = 20;

if (age >= 1) {
	Console.WriteLine("Inside if");
} else {
	Console.WriteLine("Inside else");
}
```
We can use **else if** statements after an if statement to check for multiple possibilities
```C#
int age == 20;

if (age < 10) {
	Console.WriteLine("Younger than 10 years old");
} else if (age < 18){
	Console.WriteLine("Younger than 18 years old");
} else {
	Console.WriteLine("Older than 18 years old")
}
```
## Checking for multiple conditions
We use the symbols **&&** to add another condition to the if statement and check for both conditions to be true.
- Output will **only be true** if **both conditions are met**
```C#
int age = 20;

if (age > 18 && age < 65) {
	Console.WriteLine("This person is an adult");
}
```
We use the symbols **||** to add another condition to the if statement and check for either of them or all to be true.
- The pipe symbol **|** can be written by
	- CTRL + ALT + W
	- ALT GR + W
- Output will be true if **at least one condition is met**.
```C#
int coins = 50;

if (coins == 40 || coins == 50) {
	Console.WriteLine("We either have 40 or 50 coins");
}
```
All conditions are **evaluated from left to right**. This is important when writing code like this one below. We can also use parenthesis just like in math to change the order of checking the conditions.
```C#
// this is going to be checked left to right
if (true || false && true || true) {
	Console.WriteLine("Too complicated condition ran successfully");
}

// this is going to be checked first in parenthesis and then the rest
// in this case both the OR conditions will be checked first
// after that the AND condition will be checked
if ((true || false) && (true || true)) {
	Console.WriteLine("Too complicated condition ran successfully");
}
```
## Conditions can short circuit
This can be important to increase the performance of the code, such as in some highly demanding applications.
```C#
// this code will execute after the first true, because the OR statement needs at least one to be true.
if (true || false || false || true) {
	Console.WriteLine("Short circuit");
}

// this code will be skipped after the first false, because the AND statement needs all to be true.
if (false && true && false && true) {
	Console.WriteLine("Short circuit");
}
```