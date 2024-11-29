# How to use functions?
## Function basics
Function puts code into a "box". It is good for organization and readability. It also improves the speed at which we can code. They may also be called methods, which is actually the correct name in C#. *Functions receive only copies of values*
When writing a function, we need to defining a data type
	- **void** is used when the function doesn't return any data
		- adding **return** to a void will end the execution of the function there
	- **int** is used in math
		- if we define a return value type, we **need to return something**
		- we use the **return** command to return a value
	- **bool** is used in true/false statements
```CPP
// int demonstration
void Update()
{
	AddNumbers(4, 8);
}

int AddNumbers(int x, int y)
{
	return x + y;
}
```

```CPP
// bool demonstration
void Update()
{
	isPositive(4)
}

bool isPositive(int x)
{
	if (x > 0) {
		return true;
	} else {
		return false;
	}
}

// for simplification we can also use this format
bool isPositive(int x)
{
	return x > 0;
}
```
- When naming a function, we need to choose something that really defines it, to improve readability and ease of use.
- **To run a function, we need to actually define the line where we want to run it**
## Structure
```CPP
void SayHello()
{
	Console.WriteLine("Hello World");
}

returnedDataType name (parameters)
{
	code
}
```
## Parameters
- They are **variables**
- We need to choose a type and a name when defining in functions
- If we define a parameter/argument inside a function we need to define it each time we want to run the function, otherwise it won't work.
	- We can also put multiple parameters there to make it more complex
```CPP
void Update()
{
	GreetThePlayer("Black0032", 20);
}

void GreetThePlayer(string playerName, int age)
{
	Console.WriteLine($"Hello {playerName}, you are {age} years old!");
}
```
## Chaining functions
- We can chain functions by nesting a function in another one or we can use a function to define a parameter
```CPP
void Update()
{
	// this would print out the age 20, as defined at the start
	GreetThePlayer("Black0032", AddNumbers(8, 12));
	
	// this would print out 20 too
	int ageValue = AddNumbers(8, 12);
	Console.WriteLine(ageValue);
}


void GreetThePlayer(string playerName, int age)
{
	Console.WriteLine($"Hello {playerName}, you are {age} years old!");
}

int AddNumbers(int x, int y)
{
	return x + y;
}
```