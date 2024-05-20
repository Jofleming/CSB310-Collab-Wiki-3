# CSharp ![alt text](image.jpg)

C# programming language encompasses a rich variety of data types, expressions, and assignment statements, each serving a distinct purpose in software development. 

**Data Types:**

Data types in C# are categorized into three primary groups: `Value Data Types`, `Reference Data Types`, and `Pointer Data Types`.  

Value data types directly store variable values in memory and can accommodate both signed and unsigned literals. Signed integral types can handle negative and positive values, while unsigned types solely accommodate positive numbers. Integral types span 8-bit, 16-bit, 32-bit, and 64-bit values. Floating-point types, such as float and double, cater to decimal point values, with float representing 32-bit single-precision and double representing 64-bit double-precision floating point numbers. Additionally, the decimal type is adept at financial calculations, boasting 128-bit precision. Character types represent UTF-16 code units, and boolean types solely accept true or false values. 

![alt text](image.jpg)

Reference data types, in contrast, store memory addresses rather than values directly. Examples include strings, which represent sequences of Unicode characters, and objects, which serve as the base class for all data types in C#.  

Example: 
```c#
    // In this code, dog and dog2 refer to the same object. 
    Animal dog = new Animal(5); 
    Animal dog2 = dog; 
    dog.GrowOlder(); // Method increases Age by 1  
    Console.WriteLine(dog.Age); // 6  
    Console.WriteLine(dog2.Age); // 6
```

Pointers, another category, also store memory addresses. The ampersand (&) symbol serves as the Address Operator, determining the address of a variable, while the asterisk (*) symbol functions as the Indirection Operator, accessing the value stored at an address. 

Example: 
```c#
    // Get the memory address of the variable 'number' 
    int number = 10; 
    int* ptr = &number;
```

**Expressions:**

Expressions in C# facilitate computations that yield values. They include Constant Expressions, Variable Expressions, Arithmetic Expressions, Relational Expressions, Logical Expressions, Bitwise Expressions, Assignment Expressions, Method Call Expressions, and Conditional Expressions. Each type of expression serves a specific computational purpose, from simple literal values to complex method calls. 

Expressions in C# are combinations of values, variables, operators, and method calls that evaluate to a single value. They represent computations or operations that produce a result. `Constant expressions` are simple values like literals, while `variable expressions` are represented by variables themselves. `Arithmetic expressions` involve arithmetic operations, `relational expressions` are used for comparison, 'logical expressions' involve logical operators, and `bitwise expressions` involve bitwise operators. `Assignment expressions` assign a value to a variable, `method call expressions` involve calling a method, and `conditional expressions` utilize the ternary conditional operator. 

Examples:
```c#
    // Constant Expressions
    const double PI = 3.14;
    Console.WriteLine("Value of PI: " + PI);

    // Variable Expressions
    int x = 5;
    int y = 3;

    // Arithmetic Expressions
    int additionResult = x + y;
    Console.WriteLine("Addition Result: " + additionResult);

    int subtractionResult = x - y;
    Console.WriteLine("Subtraction Result: " + subtractionResult);

    int multiplicationResult = x * y;
    Console.WriteLine("Multiplication Result: " + multiplicationResult);

    int divisionResult = x / y;
    Console.WriteLine("Division Result: " + divisionResult);

    // Relational Expressions
    bool isEqual = (x == y);
    Console.WriteLine("Are x and y equal? " + isEqual);

    bool isGreaterThan = (x > y);
    Console.WriteLine("Is x greater than y? " + isGreaterThan);

    // Logical Expressions
    bool logicalAnd = (x > 0 && y > 0);
    Console.WriteLine("Is x and y both greater than 0? " + logicalAnd);

    bool logicalOr = (x > 0 || y > 0);
    Console.WriteLine("Is either x or y greater than 0? " + logicalOr);

    // Bitwise Expressions
    int bitwiseAndResult = x & y;
    Console.WriteLine("Bitwise AND Result: " + bitwiseAndResult);

    int bitwiseOrResult = x | y;
    Console.WriteLine("Bitwise OR Result: " + bitwiseOrResult);

    // Assignment Expressions
    int z;
    z = x + y;
    Console.WriteLine("Value of z after assignment: " + z);

    // Method Call Expressions
    int max = Math.Max(x, y);
    Console.WriteLine("Maximum of x and y: " + max);

    // Conditional Expressions
    string message = (x > y) ? "x is greater than y" : "y is greater than or equal to x";
    Console.WriteLine(message);
```

Understanding and effectively utilizing expressions are crucial for performing calculations, making decisions, and manipulating data within a program. 

**Operators:**

Operators enable developers to perform arithmetic calculations, compare values, combine conditions, manipulate binary data, and assign values to variables efficiently. Operators in C# are symbols or keywords that perform operations on operands. They define how operands are manipulated to produce a result. C# operators can be categorized based on their functionality and the number of operands they take. Functionally, they include Arithmetic Operators, Relational Operators, Logical Operators, Bitwise Operators, Assignment Operators, and the Conditional Operator. Additionally, they are classified based on the number of operands they take, including Unary Operators, Binary Operators, and Ternary Operators. Unary operators take one operand to perform the operation, binary operators take two operands, and the ternary operator takes three operands. 

`Arithmetic operators` perform mathematical operations on operands, such as addition, subtraction, multiplication, division, and modulus.

![alt text](image.jpg)

`Relational operators` facilitate comparisons between two values, returning true or false based on equality, inequality, or magnitude.  
![alt text](image.jpg)

`Logical operators` combine or negate conditions, including AND, OR, and NOT operations.  
![alt text](image.jpg)

`Bitwise operators` operate at the bit level, performing operations like AND, OR, XOR, and complement.  
![alt text](image.jpg)

`Assignment operators` assign values to variables, offering shorthand methods for operations like addition, subtraction, and bitwise operations.  
![alt text](image.jpg)

Finally, the `conditional operator` is a ternary operator that returns one of two values based on the evaluation of a Boolean expression.  

Syntax:  
```c#
    condition ? true_expression : false_expression
```

Example:
```c#
    // Using the conditional operator to check if the number is even or odd
    int number = 10;
    string result = (number % 2 == 0) ? "even" : "odd"
    Console.WriteLine($"The number {number} is {result}.");
```

Understanding these fundamental concepts is essential for proficient development in C# and lays the groundwork for creating robust and efficient software solutions. 
