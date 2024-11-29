Defined variables are accessible **only in the block where they have been defined** or in child blocks.
```CPP
internal class Program {
	
	static void Main(string[] args) {
		int age = 35;
		bool isPlayer = false;
		sayHello("Black0032", age);
	}
	
	static void SayHello(string playerName, int age) {
		// this line doesn't exist in this context
		isPlayer = true;
		Console.WriteLine($"{playerName} is {age} years old!");
	}
}
```
![[code-blocks-scope.png]]
# Class variables
If we want to use some variables in the whole of our code, we need to define that variable in the class.
```CPP
internal class Program {
	
	// this is a class variable
	static bool isPlayer;
	
	static void Main(string[] args) {
		// code example
	}
	
	static void SayHello(string playerName, int age) {
		// code example
	}
}

class PlayerClass {
	
	void Testing() {
		// isPlayer would be unusable here
		// This is because this is a different class
	}
}
```