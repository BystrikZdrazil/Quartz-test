# What are variables in C-SHARP
Variables are containers for data.
## Data types
The different data types used in coding
## int
- Can **only store whole numbers**
- Needs to be written in **all lowercase**
- Can store data of up to 2 147 483 647
### Setting up
- We can set up **int** values by one or multiple at a time
- We can also change the value later if we want to
```Cpp
int age; // creates a variable with no data in it

int age = 20; // stores the data of "age" with the value "20"
Debug.Log(age); // prints out the age (20) into the console

age = 54; // changes the value of "age"
Debug.Log(age); // now prints out "54"

int age, health, power; // creates multiple int variables with no data
age = 20;
health = 100;
power = 90;

int age = 20, health = 100, power = 90; // sets multiple ints with values
```
- We can reach its maximum value by this command
```Cpp
int number;

number = int.MaxValue;
Debug.Log(number); // prints out 2147483647
number++;
Debug.Log(number); // prints out -2147483648, because it loops back
```
### Operations
- We can do multiple operations with the values
```Cpp
// all of these lines increase the value by 1
age = age + 1;
age++;
age += 1;

// all of these lines decrease the value by 1
age = age - 1;
age--;
age -= 1;

// these can also be used to multiply and divide
age = age * 2;
age /= 4;
```
- We also can do operations using multiple variables
```Cpp
int age = 20;
int health = 100;

Debug.Log(age + health); // both are numeric values so it prints "120"
```
- To print out multiple values instead of doing math with them, we use a string in the code
```Cpp
int age = 20;
int health = 100;

Debug.Log(age + ", " + health); // this prints "20, 100"
```
## long
- **long** is a 64-bit int value used to store large numbers
```Cpp
// this is the max amount of a long variable
long myBankAccountBalance = 9223372036854775807;
```
## float
- Precision = around 6-9 digits
- Size = 4 bytes
- Needs an **f** to be able to function properly, as without it it would be a [[#double]]
- Most common in Unity
```Cpp
float age = 20.4f;
```
### Operations
- We can do all mathematical operations with a float
```Cpp
float speed = 17.2f;

speed = speed + 1; // addition
speed = speed - 1; // subtraction
speed = speed * 2; // multiplication
speed = speed / 4; // division
```
## double
- Precision = around 15-17 digits
- Size = 8 bytes
```Cpp
double age = 20.4;
```
## decimal
- Precision = around 28-29 digits
- Size = 16 bytes
## string
- Stores **text data**
- We need to use double quotation marks **"**
- Spaces matter and count as a character
```Cpp
int age = 20;
string name = "Aramin";

Console.WriteLine("My name is " + name); // prints "My name is Aramin"

// for longer texts this may be inefficient
Console.WriteLine("My name is " + name + " and I'm " + age + " years old.");
// a better way to do this is using the $ and {}
Console.WriteLine($"My name is {name} and I'm {age} years old");
// both of these lines print out the same text
```
## bool
- Can only store **true** or **false**
- Used in if statements and conditions
```Cpp
// we could use it for example to set hostility to NPCs
bool isFriend = true;
bool isEnemy = false;
```
## var
- Automatically detects and assigns variable type
```Cpp
var myVariable = 10; // this would be stored as an int
var myVariable = 10.2; // this would be stored as a double
var myVariable = 10.2f; // this would be stored as a float
var myVariable = false; // this would be stored as a bool
var myVariable = "false"; // this would be stored as a string
```