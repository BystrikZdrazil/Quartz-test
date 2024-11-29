# How to convert variable types?
## Basic conversion
- We may convert smaller value types into larger value types, but not the other way around, even if the value itself is small enough to fit
- This is only between variables that store the same value type
```C#
// here there is no error because we can convert int into long
int universeAgeInt = 15;
long universeAge = universeAgeInt;

// here there is no error because we can convert float into double
float burgerPriceFloat = 15.4f;
double burgerPrice = burgerPriceFloat;

// there would be an ERROR here because we can't convert long into int
long milesDrivenLong = 150;
int milesDriven = milesDrivenLong;
```
## Complex conversion
- We can convert variables into others even if they use different value types
- This may result in data loss
- When we convert data with decimal points into data without them there will be no rounding and just everything after the decimal point will be ignored
```C#
// if we convert float to int we will lose the decimal point
float age = 20.4f; // the value here is 20.4
int ageInt = (int)age; // the value here is 20
```
## When to convert data types
There are many scenarios where we want to convert, one of which is calculating the % of max health the player currently has. If we store data in an int and don't convert, the result in this case would also be an int.
```C#
int health = 1;
int maxHealth = 10;
Console.WriteLine(health / healthmax);
// normally this calculation would result in 0.1, but because this is an int value type, the result is also an int, therefore 0

int health = 1;
int maxHealth = 10;
Console.WriteLine((float)health / healthmax);
// by converting one of the values to float, the result will be a float, displaying 0.1 correctly
```
- Some data can't be converted, for example
	- bool --> float
	- string --> number (int / float)
- If we want to convert a number into a string we need to use the **Convert** function
	- This only works if there is a number, if there is anything else it wouldn't work
```C#
int health = Convert.ToInt32("56");
// we can also use for example ToInt64, which would convert into long instead of int

int health = Convert.ToInt32("asdf");
// this would result in an ERROR
```